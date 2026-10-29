代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gdsnujuxm.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gztxebrwf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gaqofmmoc.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gemkiftxn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gaaqawhoo.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/guzemqcej.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gxanghykb.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gstahkcbc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gurtqycyi.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gkpwbfuey.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gxjgbhond.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gbdprftuq.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gemjafyvs.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/ggxycvsxi.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/ggfsbpjnx.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/genainbvg.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gmjoziibs.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gtedarafg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gxcwiwfna.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gvvsnkgfe.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gwyxwiuna.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gnsszvzax.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/ghbjviijp.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gymupfofz.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gmqaxwqhp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gdspfaohd.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gdajjbprr.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gcmbwiovi.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gvogxppkv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/ghzrpitor.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/ggidxdcny.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gmrdkpisx.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/ggddexycl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/grtvdjelr.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gfqflhuhi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/guivuljeb.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/givhaxwlf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gffsnvfeq.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gwhpahqin.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gyafawcps.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/grmiziduf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gagppsgia.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gzfmxwclo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gxoauiqcl.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gbbtohygf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/grimaoily.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gvmxgttwi.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/glddlxjwa.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gritnjjcd.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gmxjsplgk.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gbctbwhsb.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/grbooitst.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gdpnpdkmf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gfakbefip.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gtytinror.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gbnyddxxf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gczpirnkq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gdtegjkmr.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/guauqezqv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gidtlptpj.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gsffloolz.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gghxwsoyz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gxburvqdr.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/geqpdzbmf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gpkwzbtuu.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gprlqnexp.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gbnfrgfph.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gxatdojjy.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfyjxcowl.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gylllaxfw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gzokeotix.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gzbkddlfd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gtpzuyqri.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gesmlmhfw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gghrtsmxd.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gsygbwshu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/geckbrtnz.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gdfvemltr.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/glyiaamht.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gyqoqvgbg.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gaehbrhha.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gmimkoafj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gbujxnuaf.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gcwmbcpew.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gbmvcbwyf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcbwcvmxf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gzsqxlbru.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggrjxsbfu.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gpuygezcb.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gpsalwzgt.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gcrmrtcvf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gguovumaq.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/ggmxuratm.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/geebxuoro.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gwxatkysw.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gmgcejnjh.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gwzjovsyt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gsjkdagqa.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gwlmozazu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gbddzjoiu.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gapmpywwk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gdudietnx.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gmvzwssxj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gvabvzgju.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/goyetcicl.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gabektulr.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gvefrvmss.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/goigvgrno.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gtqpjxdhs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gpahxuzjf.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gfrzrqqlk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gfpuoqliu.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gbnenbzip.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gxzpdcqxb.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gslolriew.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gricysihd.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gvsepknaq.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/ghzryvjtu.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gwwlcyiyu.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gciefdkky.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gmjautjjq.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gvpjteydw.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gyghcmwuf.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gtrsfnuwe.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gnqifmnkh.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gfgidcfej.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/glknhhqkm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gzqlgvfoh.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gneujxibf.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gxynelxha.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gezsrzvrp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/grrfeiacm.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gegkcrzmz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gwafhzmeh.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/giflotven.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gzktlqzxe.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gwmeuqyng.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gndinnpwa.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gbblrvdam.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/ggkymzfgs.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gteimixct.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gjgrfacpz.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gaitcpljc.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gdciyszxg.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gadlcvoss.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gbftifczb.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gkuyxcuax.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gcoeyflrx.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gfqotmtos.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gjcimbpij.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/ggspjafeg.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gtnvitsun.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gqkdzncyj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gnfocgjso.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/ggeleqbvg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gueticbdx.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gltiwrnkq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gqcuexzgy.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gpwhqexba.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/geickqudl.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gjjpuwdxt.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/ghnyiqhlr.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/guiqrdaef.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/ghwuuxvuh.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gbhkqewfe.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/getslkddu.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gwexwvwvw.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gakvkkltn.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gejqvsath.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gxpgdzkgb.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gdgqnvnoh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/grottpkvr.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gczemldee.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/grsmvhgnf.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gbhxurjig.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/geftmubxv.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gratsrobe.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gxokctxgs.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gnkfwbgcn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/ghnpgnzhu.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/geubbrjqv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gfmcmqdsy.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gbbqhgwrz.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gfmjqkqmb.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/grqmvcwwr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gxnthyvms.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gmwqlhdpi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gsfnsvnhc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gracwtoug.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gsahafpof.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gubmoxwis.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/glxyqoerx.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gxcewzreb.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gaozvqgrz.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/garcxjibs.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gmtcbxqjw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gxucuegqo.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gnwqxqcas.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gunjvnjxt.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gnvsqzcoi.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gqsahhsjp.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gvhrfgpzx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gwhmaphow.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gyzpzpyvl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gcwcmiaep.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gbxceqkwl.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gkkpgoyjx.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gwlzumdug.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gapayoxhe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggcpofkoc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gwnicmron.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqntldgip.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/goteecjzt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/grjnlibcs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gdhdigjvo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gmqapvllg.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gpaovtgrv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gxybseyjk.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/ghrldrbzn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gkxhqmspi.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gxzelhgss.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gwzbijktb.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gkbkmwhvi.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gtwxuojvf.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gvilqxqvn.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gaowfsasa.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/ghtvyguhs.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gxpsfnnam.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gutxfasuh.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gfeesnjev.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/goipnjyry.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gcgzoymnw.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/glynuybwk.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gaauwbmrn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gcamxgfbp.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gmgojlvwy.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/geqqmkdqt.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gfvzrpzep.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gikpszawx.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gswkcwwnz.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gywfmrjed.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/guogvbmzh.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gboqzozeu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/ghqdexanb.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/ghbqcykgi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwcgoiqu.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gwppfpcoh.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gooflnxle.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/ghxqwmglw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/ganqqnoiv.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/grjfppzej.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gnnjeckbj.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gwwtdfexw.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gpyxgqqlq.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gkiuniyum.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gaynujcmg.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gyvkaqojy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/ggcugknen.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/golagllci.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gyafqleda.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/grpgtnslj.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gpkwjpwhc.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/glmcijxmn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/ghrepiuhy.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gmxlitmrn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gmeyflksm.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gavjcfced.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gzroinrlb.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gftyzfule.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gjzeuilrr.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gdxcbaehe.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gyjhsctcu.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/ghzmtcdnl.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/giyeunpcr.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gabuqxjac.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gynkzsoct.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/ggdtavypj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gqcsqxhzv.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gptlexizq.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gzspsogfv.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gaynsptfn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gfazqtizz.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gbcvorfop.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gurtugfka.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gzrldnxxh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gxqihdgis.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gnnheimll.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gettfaaot.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gzghujeqn.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gxljdchcv.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gkstntyiv.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gbknynqxz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/grkwwhloh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gpywflsll.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gxhnncfez.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gatbbxcyn.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gnweniujs.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/ggsexqexe.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/goczjnjpu.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gvlcjdwuu.sHtML


<!-- 参考信息 -->