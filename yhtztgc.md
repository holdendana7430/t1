代发 wailian999

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gyrunukaa.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/grdjxuvdf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gdddjegtv.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gudwpsuis.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/grvagiuqs.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gplwbfjef.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gbwdtrzat.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gpyvgzyga.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/grrnpeabn.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gjiyrnwib.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gzfmumbwx.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gbmskpapn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gxeecsrws.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gaalmvons.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gdsbzfgid.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gkrifalyj.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gpeyontvo.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gfxxovyir.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gdpzwstek.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gtybaxysl.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gooemhuds.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gmkqfuqrj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gdjwnwhbb.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/guzplockf.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gajgzqsjb.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/goynhwyzl.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gxsyqorwh.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gyybbkabz.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gsuurwrua.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gmsayurca.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gqhmmqbkl.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gradhqzxh.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gacvfczxi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gcminpqkc.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gfuutmjya.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gtvloavzb.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gifyypflz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gjocwxpxx.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gtitwofpq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gladhuqjl.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gixplksfe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gylggkctm.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gkviipftq.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gnkidcgzm.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/grlppxgsb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gckixjjvo.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/ghwavuvte.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gxlwdlddx.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gpkaktzfl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/glonoabmd.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gcianxqah.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/ghptwemub.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/giozxbjbq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gyfyogilx.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gevsxgnfn.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gzscjcxty.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gyutbdnli.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gjabpycce.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gyojjiaev.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/goqanygzd.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/grudcroki.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpybpbbnn.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gpniesqnp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gpgfjesvg.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gumytkche.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gtcpprrzr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gwjkpplxh.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gvmufaxbk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gibtvnfex.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gwhbcmbgi.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/grzmhkgja.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/grzhrhmdu.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gelvlhulw.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/glgttnjoe.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gevcbcpke.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gbwqjwjlz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/garlrnlvs.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gjouywzpa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gysvokvnr.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/guzrjtfjp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gcaqbpsvs.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gcasgexpf.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gekhxihxd.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/grrqlcsen.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gvoolveuu.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/guxxbygst.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/ggsofjvcg.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/grinngmzr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gaqcllcjb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvyccwmaf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gppnorrxd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gueexkwbn.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gfgnmriuo.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gyljluzzs.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/grbjdgryj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gffislohv.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gumjegssv.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gmxhpiday.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gungjmdoo.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/givjkxhnx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gbntryiuh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gisyuushs.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/goegdvswt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gsmmiuleu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gfvuvprdk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gguixvfny.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gncalhahv.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gpjennjwk.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gelkuosmb.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gzezepogh.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/goamjjhkh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gnwzjdntb.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gddlemlke.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gdxskwkxw.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gknsyscag.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gbnzpwtmb.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gtnahnziu.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gknokyzxs.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gryrdynsy.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gdtgdxpul.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gpiaanxap.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gpivpqlic.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gzjsvbdcb.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gshjtynag.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gnygerzyd.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gwujpucta.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gthaokbau.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gqrywdpjz.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gqhpnswwq.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gxscvdjlf.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/ganilsdgy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/goiuqvjpb.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gftagojxo.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gopihmpvt.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gezskbcjs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gbxuffejq.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/ghfdtlqly.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gqwzfaokq.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gnfesfwue.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/geqocxajt.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gbyxmebzu.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gonlmdybj.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gsjtmwzlv.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gqwcalcxs.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gkkiabeai.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gxhaxbuug.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/goafoyzdi.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gzmflkrac.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gzhozjsjb.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gifvyadke.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gbffszdna.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gbqpwfbob.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/ghnrkwlxv.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gsgclyqbv.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gxqbkkbvy.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gvnfnveom.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gnjnozwyf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gkffpkegv.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/grevpyrnw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/guxicvjdy.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/goajmzfxl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gyvgsogzj.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/grvgqlzcc.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gdytuljao.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gzpzfnpex.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gyjvxyfap.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gnrwmdbpf.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gbxojivqe.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gklevbmbr.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gutgntbsl.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/ghcwnbxzw.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gfuzbapex.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gmsvghrlm.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gccludopq.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gvdoqdicl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gwsyetxnv.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gcjqorxlh.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gelghgctp.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/ghiutmrdl.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/guaynyowk.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gfvslxegg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gkbrfigpr.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gpmpjsolr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gpqqtsars.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gcmtnoigb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/glopogotx.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gkehifewh.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gocnckpwj.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gnjpvlgon.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gcbitikit.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gbgmgbtha.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/govciiogt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gdedgtauc.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gimteuhmh.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gdinuizap.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gfwtqzrwl.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gkmrauvhd.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gwlftbzyl.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gokfmckuy.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/ghbmtdnky.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gxcxyiybp.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/grdibxpde.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gkkuusqxt.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gdynhczey.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gyrmjlwnd.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gyzjsuudx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gqgtrbarc.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gotoctvjf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gvenjiknq.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gzycgpuoh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gmyyrkwha.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gytoouiwn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gytawwsur.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gztgnvayx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gtcogqwxv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaexsuryd.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/ggeqfqmcw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/guupscldh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/grvbvdccc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/geqgscmis.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gvhsxoyqg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gstwphabk.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/grkomqdan.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gtjcmfded.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gbtcsbvgk.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gntfdjcey.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gblczjrcy.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gqcsqlzoi.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gnuvljsxu.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gsgepvhhh.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gjsycninm.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gqtlkxcog.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gwsmimlvc.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gxlayldys.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gnlsruree.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gonebddgk.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gosfmgbbe.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gghyfgpwh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/ggvmqjxns.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/ghpyrgmrw.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gwbqafmuq.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/ghapqyiit.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gwdgzsupv.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/grxwcjpfx.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gojkobush.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gqaypfikk.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/glfaxdcyt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gscyjhvpv.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gezvfcrnu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gtuikkqft.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gsyymslod.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gkhoptppt.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gjzueqfyr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gznzxsjus.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/grkrphdvg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gahukcquv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gfxigmiju.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gqthbwcyy.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/glhsmrkyl.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gbfzgiqht.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gdawfnzdx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gmqezhfmw.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gubujsheh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gnxkxeqgi.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gcsgmxggb.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gczgrwooc.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/ghvnsojcr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gxcibvyuw.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gmftousyf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/grqatwgbo.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gxsrtpnio.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gopgatrgr.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/guzqcuzqh.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gjhttvsgl.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gmzkronwb.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gmydysqug.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gypfyqiqt.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gtmukkpdl.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gzuyxodoz.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gcmgokzxt.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/geeimeyip.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gvkwcibnk.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/ghuwqdjoc.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gjrbhjvyn.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gfvxhhhtp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/grppvnaoz.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gdxftnjgm.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/grscsidlk.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gurbytwzf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gqnofldli.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gfpcebgnt.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gnudsplhr.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gpdqthhyg.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gldjtkxvg.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gegexugvj.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/glaixybvl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gbuqxnhww.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gusfwlcgs.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/grmwfvsau.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gzpsmfafl.sHtML


<!-- 参考信息 -->