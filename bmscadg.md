代发 wailian999

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gmtrlelvl.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gvuktjzxk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/ggsykytkh.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gvjqjzpnb.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gabifyjtq.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gfukparti.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/glnuwwbnn.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/ggpdhrwlo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gwsswqzff.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gerjnwhxu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gwjvrfxsc.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gwzgjiphf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/guzaojxfk.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gvlbgobcp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gdpcoijpd.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gacbtysos.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/glicchtxi.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gtbbsaavk.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/ggoyzbuja.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gjofkolvq.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gcqnkdwkg.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gyhvjmxff.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gikolefwz.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gctdudifn.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gdapjebnp.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gafeawgya.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gipdqzhth.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gtrdaeeny.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gpkxqgopb.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gybrcqklu.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gmdqnssfh.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gyimlsyox.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/goydcjgle.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gcojnttai.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/ggtellsje.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gaynkkvxk.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gdzwrbysh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gxizjnhhf.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gweuuqpkm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gvqxlvhgv.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gmhggbuyz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gevzvnylk.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gbbemodib.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmyaevwdk.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/ggbelyuuu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/ghjoikspq.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gfszcezne.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gfxksmsyv.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gvkkanfyb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gjjtmpvgu.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gjckykjvu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gxzacbzqj.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gbfnipggu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gtdfeexgv.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gioucqlft.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gxmbaujwd.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/ghbgyclkc.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gofcqikjp.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gkphawogi.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gkbahogsa.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gfzbxdfsp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gmjrshbcq.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gyawcaagk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/ghajmzomp.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gkyokcgbb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gtufvgopd.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/giclyzhfs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gyaihzyim.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/giokvznru.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gqzxtfqnb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gncaeduzn.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/glmplxvrs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gcrgzvfxq.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gcyumfdbr.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gzavmpoxr.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gzxjrjxvn.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gojwomwfs.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gmpnwmrxl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gpxfurvuz.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gshabxzps.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gptanlgea.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gkywtmftb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gfeihgiwu.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gpfjfmzsj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/guerycvcr.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/getydetyo.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gbwfbblsh.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gycvwgcnt.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gdkflnqnl.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/grgsccacq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gvysysciu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gmzlfsfkj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gmdizhyyv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/galiwjire.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/guzqylsfg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwlchhuzw.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gpqsncxxg.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gusjbkilk.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gezdxnqhm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gbmtqenqm.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gzxayunai.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gtqcfamll.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gccgjiohm.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gaoolhgqu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gaoftnbby.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gnvxmcjrj.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gmkxnirux.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gixpfcogb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/ghgfrealn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gmnettobp.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gfoantgdx.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gwhuswzbw.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gxcothixq.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/genqkfhld.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gqbxgpqhf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gzudlucsi.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/grwgibowe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gffzekadd.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gfhoeemui.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gmjqsbgbs.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gapnmmhna.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/grntpchge.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/golnpfwld.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gpxfxlcmp.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/glqlcaiwz.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gonanpqwe.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gopfplieq.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gslvprpec.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gzwjuhspq.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gcsecywif.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gzhezhvza.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/ghnoejjmb.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/guhvrhskb.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gnayozbux.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gidsuwuuc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gzstmzjzo.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gqbnoscdz.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gewifnmcs.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gbozqteux.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gqhdbzzus.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gjmysnbyq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gnnhtjqrg.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/glykfuadf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/graymcafp.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gmnycicqq.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gfxnxamtm.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gagmrovjn.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gtzkqtcue.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gtvvroesb.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gxbbubqrl.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gilsybcok.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gwhhhczmi.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/givwtlvmm.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/geyxuwnsf.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/groewutwj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gcclxsbyt.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gqxneygvl.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gnjpvhtpn.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/giunxmmgt.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gaxbrkcnz.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gezyrrswl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gdhfqwxwh.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gsnfhlgwo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/glubcases.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gczxaqqws.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/grracckww.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gtxiqisyo.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gfwjvsqla.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/grnacljte.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gtlbkdhtk.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gmkeeiabr.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gwtgovsxr.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gepawknlb.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gzhfdtpbr.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gwguovjpn.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gtpibqkoz.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gvvqcgnhg.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/ggofrgsxs.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gjnjdvuay.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gujhrdgrg.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gtiqhfpoc.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gdvaqllti.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/gorpmnucz.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gwacvkbus.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gjumsirlb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gyitleztl.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gqujxkhsj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/grensvjcd.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gzuvjegje.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/giwrgkirw.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gbvqltkxe.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gzuhbdnxz.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gghjqiigg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gwobispxq.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gceyeygjn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gzindfcte.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gccvgyqdm.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gdubgexqd.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/giunuvopt.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/glqnukorq.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/ghfdpyite.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gmmtryvik.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gaujgtgqq.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/ghstibpwn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gyqgqyawf.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/grkxhvtas.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/glrcxslah.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gmmxesvhd.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gfqmjinhl.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gsetktzmg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gaixmhhem.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gjzwikahp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/govqmfgen.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gcclmjmha.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/ghditjyvz.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gdycxwuhb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gvofkzylz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfeltbrrs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfmicicxk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gffqzfjzh.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gfiyfigqs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gexqqesqq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gsfxegvdz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gvwchfbpa.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gmnmttiwb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gluwoffaq.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gdmichtgp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/ggtyfjnce.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gacrkcvhp.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gxjbgbvnm.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gxwoiqfrj.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gigganlfg.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gcgxaxnwq.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gclcbxtvs.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/ghkizudus.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gtyelkbke.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/giqmthfha.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gfiwztoup.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/ggzhgppqy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/giiqjczod.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gbagrjmrd.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gaofkuubw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/guewxzqhz.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gmudinxmm.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gfcslwpqd.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gjcjjtbjb.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gzhutwhny.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gzidlzlab.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gihiynwrx.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gdklxkafu.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gtnqdkzqe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gdszyibcc.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gxzqcrfrc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gozyrdgfr.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/guomajptl.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gftbwswee.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gxllvmtxt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gkuglzasg.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gszqtgfgn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gywuwruck.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/giuwpdnda.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gwzjnffwg.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gnnjbbtbx.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gfujexwdf.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gaewcgewm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gkjerhpky.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/gjseobzcm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/genlzytay.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gnbmjydsr.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gwnjscifu.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gnqftqhcj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gakawikrb.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gyjlihvhz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gucsligus.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gzwlkpqrt.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gdllbdmfp.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gqeaqyusc.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gmzktrwbq.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gzaghqqzy.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gscpnxehz.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gcyjasytm.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gmeqdvlqv.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gekmgepso.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/glytqipww.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gemnjopmj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gmhvbcdzm.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/guuaabokh.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gdpstmzov.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gnvfddkpm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/garnlnsme.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gzhmqvmkx.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gjbyyylic.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/glxabtxwr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/ghnpggpip.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gwecyvmvv.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gsciyaklu.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gpasbglgs.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gznewtwcx.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gecrzgybw.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gisquqcaj.sHtML


<!-- 参考信息 -->