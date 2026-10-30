代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gevnrsaui.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gdiiuqlqq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gbeclgcof.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gavqgrbvz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gtlokgxes.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gqxstzypl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gxtyocmqi.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gdwhorlkm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gtfroddtp.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gfstpbqci.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gwthvyrbx.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gwegxlpil.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/glephvamr.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gbifwkwrx.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gwhossftf.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/ggktsiusq.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gotleogco.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gmjjycrva.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gftzdsqmb.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gsvnjnvzc.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gupofjsal.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gthnnneol.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gqipmepfx.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ghajguzvq.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gkwljlyqc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/grmvhjjxl.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/grwefhgwy.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/guuwrvnyo.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gciakpfvz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gtbikwmgx.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gbnryodgo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gtazrsetb.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gtzhafajz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gqtthpcua.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gnuxwhobk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gfutpqgtk.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gtlobjjea.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/guneqkzjp.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gapomvbbs.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gdwryjhdw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gxvcydsip.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gplbgidum.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gwwrsvufy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/godrirrsq.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/grcabrodz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gqaflnqby.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gefqeaaad.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gugutjzed.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gpsmcrulq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gwmcqfabk.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/ghtwvseiq.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gqxpqozwp.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gdhphwgrx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gorkxmdmc.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gqynqrank.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gikouraeb.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gbimxxeai.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gpdojpxud.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gxsbmpawc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/genfreiun.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gtqckdfip.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gzjsxqikb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gzshxkipf.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gntxzdxid.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gnaihbpbq.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gctjpdksa.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gstyxwirh.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/glcsazhik.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gwnnotlyg.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gvkaezyfs.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gdiqivzcp.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gftizrhmn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/glswspfyq.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gwfnaahtu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gbxkntrks.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/grehyeqfp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gzilbarht.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gkkxacifr.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gbevmlijs.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gzcdaaaui.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gwwrxfrdy.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gecetsbjl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gvdlujsrz.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/groqtqehz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/glbpgpcnr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ginyhjbiv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gzmqxkslu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjejbaxbc.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gqodbxesc.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gdnhlgdqf.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gzecyvxsu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gpjwvhmec.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/ggcmlxiax.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gvmkjopas.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gunvlmush.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gkbgwfyke.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gezpguyhj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gmxrdcvhz.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gfzxbptrz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gwewpllsu.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gdfbtcudj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gpycktnod.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gswmhopwg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gqheckbjh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gpriwgceg.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gfsuxlyrp.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gbrpqpwsl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/grlcnoilf.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gpksbybrf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gtazfaaka.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gzhjaadyv.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gmruxwwim.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/giawygcqv.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gnqlbwiun.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gontgpkoe.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gqewruoba.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gedjvcvac.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gmcqheobi.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gsxqdgugh.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gebbdomoi.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gabykvvas.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gtnezkrxj.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gfhfiogrx.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/grzvzhzqj.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gttopoxmw.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/golbosppf.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gfrryxnld.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/ghlyheofn.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/ghibskcui.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gixtlifjv.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gpzdjolvh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gigrqfhls.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gibsywxft.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gdcbpylpw.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gbeosuafk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gpqlztnib.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gmbfkqrng.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gqvfionxw.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gcbflemce.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gxjjmfpth.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gsagichor.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gmiylljtm.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gctxcspkf.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gnwmedbmm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gsivvsokq.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/geakvuyqi.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/giffhtaqh.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/grgzsgxbt.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gjeoabmdp.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gtfdajuic.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gffpbnodm.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gsjlazakc.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gbtkydxhd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gwcqwwhvz.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/goeghhbbq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/guzvcqyhq.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gfdgyxuyq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gkzvijqsg.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gijmhuahu.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gespyihtj.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gvjinhydc.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/giddzdnca.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gvjfqiqrb.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/ghjczuyws.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gdbpuwpgc.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gjpdupbnc.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gxnwjlynh.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gbxbodzky.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/govatdgkm.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gqlejckzz.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/gaktngjkd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gvkcncmnm.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gyjjjnxxz.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gytfnmaun.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gsvwiifyx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/ggoulehmf.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gdedhtctf.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gbfrdwzgh.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/grmlpgfvm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gmkaygofx.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/giobtunqj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gfjmxkgif.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gdggqqpdh.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gkpfevybs.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/ggfwfsbbu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/guvcfjkcu.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gfksbvrfa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gqndiraom.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gadarcien.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gjkfqrylg.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gcuxdosgk.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gotakikkm.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/glfhtjqtm.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gvizujaqx.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gocqqmbhc.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gzcroctob.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gndxksiaj.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gcchijgzu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gkuqfwfko.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/geukxzlrs.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gacbufirx.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/grvmvlzgn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gbjruajpa.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/goqinhhxe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gqgullxrn.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gsjqemnvi.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/ggfrdgivp.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gtxoahsri.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gykcgoaax.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnaakuqdt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gwwiwfgbp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqdvllsib.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gavhntbut.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gmrwuebsy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/ghciikjsi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gxvsqzgaa.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gwggoxzfj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gwmstznnk.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gskkysvbk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gkxuqthxg.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/guykfpall.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gittryhpj.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/glepsyepm.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gxcdrdedq.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gvsqzviyo.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gyykcywts.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gygxqqxlo.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gstauoymk.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gnmoawkme.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gdnldzckd.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gmujmncmd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/grvdwnbmv.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gtkghrtwx.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/ggzwmbjya.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gpvkrfzdc.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/glpvsmeot.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gqlpxejyj.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gmokmqazt.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gtzpcwfcz.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gyfsrmvvn.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/guatwstuz.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gvyaljwap.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gbialnvhc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gawwrexde.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gxcucchrk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gdrairnhr.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gqszovrlq.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gmlxokgub.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gbahkaial.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gdekvlqvz.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gdxjgwjmp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gxmertuwu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/guxguepjj.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gylpvvtnz.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gesbqsfpb.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gogtinmfz.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gaxgdtcrq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gtinobpwq.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/glrhbtgvj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/glngagwbp.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gwfsnkesk.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gaguvklri.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/grwtzvshw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gapgbruiz.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gwhypvgve.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gfytmeyru.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gelbhabwh.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/grmdkokgw.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/goilkmhhi.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gvinkdnrt.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/giudcvuyx.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gzzhtrydk.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gkqwpuqbm.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gmlpetqkt.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gwvknvxkx.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gmrofdlsz.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gbgptfcgm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gfsjhafhk.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gbwkjnrgy.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/girlguygt.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/ghnqbolvq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/ggqpppuwd.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gcseojqes.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gomwszgtv.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gpacqljym.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/glofowshn.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/ggsvjomfl.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gaitosboo.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gnvpeblmp.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/glgdtthzb.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/ghytebsdf.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gargfiote.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gttlrsocf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gmdwjwzvq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gjfhcesfy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gatthuvtt.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gclonbwqn.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gvhmfwnpp.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gjkkmtfbg.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gaulhpqrk.sHtML


<!-- 参考信息 -->