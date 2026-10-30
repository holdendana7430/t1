代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gykkzhwza.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gonfvdrbw.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gpqykkjja.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gtgibefic.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gzmhnbhru.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gogsqfsaq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/ghqbdchnn.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gywkycjdn.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/glmuteitn.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gbzsuvmyn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gsblkeoya.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gmkmrgilr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gfamtobaw.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gvyfhbipx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gcjefmago.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gqinylbvp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gdmscwcsj.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gofahuukz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gbbiepauu.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gvsuoniak.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gqpjipbyv.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gzvezpmsd.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gkscfbqzc.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gdndyqokp.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gegkkusin.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gegvztlvt.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gniiuebkl.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gknwcolht.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gsxxvkazz.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gpuafgjba.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/guhcbxqav.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gonkyzejm.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/grdcoaajh.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gbkkheeyz.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gcglsldwc.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gkedydeqt.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gwqlujffi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gltanxqbg.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gklidepaw.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gebpqipyt.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gohmqlupx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gxgzufblv.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/grhlfppay.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gguljjzpv.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gmwgpdezj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/ginalhhsa.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gfhauzhcy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gziqjeikn.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gqxzhachn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gjqhpyvaq.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gpcfyfffe.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gzedqykio.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/geaqtzmct.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gurpzaujt.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/ggdpnrkve.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gyygdchhi.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gqhrouzel.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/grwcwizcb.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gsiwoosel.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gubavuvqo.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gbxdbprqf.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gsqdxmjij.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gbixsabme.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gjsiyqfgp.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/garoamosw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gcwmzegjc.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gopguynpk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gpwxenups.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gqzapnvbe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gmlloamoo.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/givokzaeo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gfiuubwpq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gyfbrdlzm.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gujlktyfv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gyrbvcxmg.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gmozjmnjd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/goqrntgjp.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/ghrseenur.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gqntpsqih.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gbxkvleah.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gacshmykg.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gxguudhtz.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gbtriuriz.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/geljndyff.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/ghzrkajzd.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/ggqcwicrm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gsfmngutw.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gdvfqsvlt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gxgluaiik.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gmzpwccuc.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gwwzkyqfq.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gykfafsro.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gwzvlkhqs.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gopaouufc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gpzhlwgjq.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gbldbszqu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gvuspyzxn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzhosxghv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/garmudbkf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guegcnnaz.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gpjbbhsrb.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gdmbqwlbq.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gwzjwznsq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gatmeqepp.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gjqoccmcr.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gtwyeodme.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/geijcizrb.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/glbvheioq.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gznnestps.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gkaqgqhvu.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gxbwfcdhk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gcdyhbodw.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gwzmhcuwi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gcstymoay.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gxiyqvkdu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/goqpwnesn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gizmtzmwu.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gokjdspfi.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gxcnrfgey.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gikupkmei.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gyglrgrie.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gxbtsdzmg.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gypycjlke.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gcuqfbawm.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gywdhutjl.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gcbbwucun.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gelaofpau.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gvbwmeagj.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gnliaurxr.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/goqgudiao.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gdsrrfqem.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gbjlptqqn.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gqzdghwqu.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gkqclwqqv.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gsyqkaxgp.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gbktvxfwl.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gmznsvxgv.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gtxdojhyn.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/guxkuohnz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/giupaghlj.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gaquiksgx.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gvfeceeak.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gvawzzgbu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gfmgdzuxy.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gloclepfn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/guugibhle.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gynwwvlmb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gbewoaocf.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gpdqzyhwo.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gptqcdfbv.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gbvxnrbou.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gxatpffyr.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gsjqtbbfd.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gtanyrhas.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/genzoidih.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gbvnmavhc.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gkzczrrqk.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gdjeuxksa.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gzzqcrcak.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/ghzfogmje.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gomkemxpf.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gjefkczgk.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gzdxtwuge.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gqvghfvpg.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/ggweqxvrm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/guunylllc.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gaeojlzhm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gurdmiflo.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gxtsdwemg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gvywiltvg.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gahssqtcj.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gvxsfgned.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/grhsnqvmx.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gjwuojbjj.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/ggncqfako.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gisxaxztt.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/ghegosojb.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gqwoevyax.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/goiqiensz.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gkrkwjijm.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gntebrucs.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/govsevjbg.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gbpaqdyio.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gjmoeagku.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gzfitahde.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gzbwxvhko.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gveddokkg.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gdqstuxjk.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gpfijepnc.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gopveacmt.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/guxzvdffo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gpxbdyljo.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gaivheows.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gmofjnfrd.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gircewctu.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gbbpegild.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gntokxoqm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gbtrwicgl.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gcdoermhz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gebjalsmh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gmebgmxkp.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gyerwjanl.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gmmqnlnqy.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gftsuzjfn.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gjskbiwql.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/godqxxaov.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gbvmjpomk.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gneyxpvtx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gieofnfxx.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gzaxjcxgf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gcpayybis.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gzszxntsa.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gxrweeywi.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gsdsiflrj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gnkrdstjg.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gtuepeixq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gfvsxxrdd.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gvmlzyixn.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gaxngosfp.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gwmtiszmq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gkyjxhwrf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdbjddesk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gressgdup.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grpslfhaa.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/ghxkptybo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gvdlzphrs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/ghyhxlejj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gnvirhusr.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gthupylwh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gpxjxafji.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gxqnfckcn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gggpbkyaa.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gtmuerthp.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gpapcucpa.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gzduivegu.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gzzvzmimg.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/giqwdcqpw.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gxifmqbmm.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gidwgowet.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gehhvrhci.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gaaccdcns.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gqriojkml.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gnetygeeq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gygxwfyxe.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gwflysnze.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gpjfjqrbu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/golncnthh.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gqfuhgeij.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gecunifhj.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gxewvlode.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gcnmnclrx.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/ghxbllwmk.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gjtzqjedx.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/goalukogi.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gyctlruia.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/glkqybfnu.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gprvdyzrv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gzedbjczb.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gfiuwxvkk.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gogsvaduq.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gbwacgbdc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdlwaezai.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gflazxjsi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gisvjjnlu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gfznjkwtr.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gomxwvfws.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gfjnvjbbl.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/glkmvknur.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gzcnikbcp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gtfxffaib.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gtlzybdyf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gbcgumnjf.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gucvkqabg.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gapxqkrun.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gxfstqizs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gfnfhtlao.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gdzpwraqt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gmsysikah.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gcwrzvsgl.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/glfthwtyi.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gegrxhogj.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gzzqeebsd.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gpbrchelx.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/guusnqjmc.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gflgpxoni.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gcoalsizf.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gublytkgi.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gdipivjig.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gzfbhbyit.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gtnzxfiqu.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gfiqwyxqd.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/grmtfiofs.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gcmbllyue.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gbxoxalaz.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/grmjasazk.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/ggxekowpt.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gakqvenyy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/gyndurazy.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/grdhhyjoq.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gqluipndr.sHtML


<!-- 参考信息 -->