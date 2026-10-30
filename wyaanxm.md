代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhfsjurr.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gapolvkhh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvninpmv.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gvoszdsjv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/geiyyebea.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gutfpnaik.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbudqfmek.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjalkoawj.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzatjpgh.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gbckikqra.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gaitdcqzj.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gklgzxxiw.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmrziwuk.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggpjezusb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/ghxehyify.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gcscdnpfi.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxmgcngi.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gshzemnfv.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsoiishj.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuolnjur.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesybivos.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdkrhxsvk.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gprghisql.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfrzmciw.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gvegoydoc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtocovymz.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiqemprq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyzdaidg.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghibogslb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjwdkdwl.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gfgojkwep.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/geabncsxt.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqnpkgsw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtigxypt.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gkzagyqem.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhvruhcl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzpsjdxo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxnbdhko.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzbtayoy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnxnqyih.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gxyfrjrzx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/geihktqyi.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnzsyiyv.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gbggozsmb.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbrvklyl.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gladjvwuu.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxrnkwau.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gshhzydht.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gprvfvqmk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmzzpyjc.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gscrtaeao.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjsofwci.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqvcmrlr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgkcnrqb.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcfmvntnf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gxafhdeav.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiyunudt.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfefjdnuo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gefvnmypq.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gghkantys.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gyckaxcvw.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmjwmdlz.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnureugwp.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gsdacmphf.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtwdygdt.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/glivipcbh.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gzntwognt.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gffdetqas.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gfccyvtxg.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gwxfxbthp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gcqmglhyi.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwshufqqk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjnwerzl.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gygrhkocw.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ggoodgzqh.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/guouvfbrt.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gqwutlhqj.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/giiicaqpz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggshqdlos.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gzkrufxms.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gsiqbednw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlqiqyjn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gnunwizvg.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazusnnqr.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gzgnmudkg.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gkhgoojwm.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/grfkccwcd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gfqdsiclf.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gzvmzvwvy.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmcbaojs.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gylhjdvfc.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjrladhu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaczmkazu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gvdmutgsd.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhssedzb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwdbvovn.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gvkkuyabg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfobdenvg.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkmbpqau.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gimaqlgip.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmngkjiv.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpilxyasd.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvqpjczl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/ggxmbounz.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gqopultgh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjcakmoc.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsvjelwb.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdulzlips.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfiporsf.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gbphdlkcq.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ghltlropj.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gqmfvwqyo.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/glssjjnxo.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfucihes.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ghcqqpxmf.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gqulqcmab.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gntdgiivp.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gtknizlcz.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gugxhbnfm.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngeppsaz.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvugvzojh.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhcvxjtb.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gimbrircd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/ggvchoeai.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gtmvpflzl.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/girqnplru.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gcwallyac.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtijyvzdm.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gojmsfspa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gxzpnennd.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/garhimoam.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvuohtqb.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gprjblkha.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gxfmpkand.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaohjwar.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlarzncm.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkxbkxuv.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/geayahczl.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gfmcqtvwt.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gayhbgbiz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/grepgiiuy.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyraveyvw.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gvttcowgm.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gzzcmptnj.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwzopgtf.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/glgxirbat.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/giqbaggcy.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gllvlkwxq.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gjibibgqp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gdumtabpm.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvrtxaov.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gzgfvitmc.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gfwbmmbme.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhkrpvzx.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzdzgupi.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbkeumgc.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gbhyflzap.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gagtaeohb.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/glzfmplep.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gzbbxbmkv.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvzqqxuj.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gkpdhmjhz.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxwnpmiq.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gvtjysrkh.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gunbmjiru.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/guegbgzmy.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gftasbmed.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/goiksmied.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdygxrwii.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/guptxzbnv.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gybifkhjz.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmldkpvtt.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/guzeawxqu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goccawjrf.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gsoaszwhr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzvgervw.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gusktwrtu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdantbmty.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxvfcugp.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykzszyqx.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjpttzuzs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gybjjowme.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gstfugyht.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfrsxmqp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnhrdggk.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gkumcqqzg.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzldmeqz.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpzmdigy.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshwxphuh.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymgsgqwb.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gobzhgfvb.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gukljozmy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gqqzbjvhq.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnawkbsy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/ghjrgsggu.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gwptmjrxg.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmsbqxbd.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gqindmdkj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gknusxhlw.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gljaqawyg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gfmxidrni.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gecehiapt.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/grwfvqbyp.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvinyukq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjodghgyl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpaofnpn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gfbgvtsih.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwereyvkv.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gflipbarc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/ggakwmyvv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gdeikyuew.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gtwazdekx.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/geoxekqgp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gdkbfkerx.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngtwznkm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gqpdlfqse.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwwxwnca.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/grrxjwect.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gsihaxuqf.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoqxlncx.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gbecvbqbd.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgjwcmwb.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gdytetezf.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gzdsndsqk.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqbsgsiq.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gwyeuobas.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gncmtbtho.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnetduqpu.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgdjzzjb.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiwjzbet.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpwbgchg.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gbbhfudrz.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmpnamaw.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/grykoxyic.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gegkrqdgs.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqexkqblc.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeprawdc.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gwpurshjk.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gfodjgosv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyazggwue.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/glttvilfh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gggrquknz.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gfyoniiwo.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gxfgcnnwj.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/grvzbeuoz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhyuphxj.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gaagvioew.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gbpwsuahd.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guixfqzsn.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gfwtaqihd.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gvgriwned.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/gexzlzzil.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgmuufqs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gocrfxqzc.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrdpdkzb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlojcfes.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/guhhxerns.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfittcpcf.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gykeptkwm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/glkarkhrx.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/govffdbmd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcwfqchd.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpmqyzho.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gzdhddakj.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gvbrzrwsg.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjticpqz.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gafhgxgjp.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtjrwjaf.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gpriuhezd.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gqdmjudli.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gurjxhyiz.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gnrfprkrj.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gqnupluml.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gnqepuext.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gkktqmvla.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjntjiwbq.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjozwsmr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gkxhegoug.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuiaojij.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gbnchlals.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmudvbfrl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmymosiux.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gnngwdslg.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gphelsnlv.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gkybljcbp.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gsfwwydun.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gkbulcfie.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gmqllwwpi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/glradquzm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxbwdyvs.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gweodwxlp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfdppful.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gfdpfgmkj.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjfrscbl.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gtznechla.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/glmmqrjkb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gvucxltru.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjivlxej.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsbdtiki.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gitykhyrm.sHtML


<!-- 参考信息 -->