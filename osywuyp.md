代发 wailian999

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gweewdjgw.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gbpoxphcw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gklgydpyz.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gojuvpnnj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/ggxykrqak.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzatfpepi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/govmemzfk.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gypmdhasw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gynpeosrs.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbctvtfki.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvoyirng.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgggutvx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwxtwsgk.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxykjsol.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbncgasrp.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/garerbibc.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geismbxtj.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/glvwpcdkl.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsaqojae.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfqauacp.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gphalbrmo.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzrjpvxd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gawhuspkk.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gojicjdvk.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gagtwqduh.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gnlzoloig.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gjkhabkzl.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ghfjhnvih.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gydgswuah.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwkvmvaax.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggommdyhb.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gozjogksp.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gpthrdvsr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlcvmtjp.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gynwkxxam.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjrasgdp.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsnxdvny.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gvtrtziql.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gqtkivylu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdqyspqah.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gasgrgzdd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/giqzbcgdc.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gdisiocey.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gbafztsks.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gmxbmbzln.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyxwgzmv.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwhjctnp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqegvcng.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwiecwmhz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gusqibhjw.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnfqqhfes.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucuvclru.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdfexsnj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcytepaa.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvxwdzly.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyqcazsp.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/glpiqdcej.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gpysvrzkc.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsmkhwpm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/glmqolkby.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gjcwhlzdu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdykxxhsg.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/grrhdiydj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjscrmoxo.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gmpwfzgaj.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/grvkatiql.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gthibgeng.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gbbfgqxlg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gesvsvkgc.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfwtnnij.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gifciswzs.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gvsdrrsso.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdvxhhjah.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gsikpwehx.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/glfrnkjlf.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/ghncxuzul.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gucfwdmph.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gqipglbti.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiaroocz.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gflyvghci.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxbghktxh.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gukgclruy.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/ggfxeztzg.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gsgusspuu.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gmbckngei.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvgfzszs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/goemlymqx.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/geescxqen.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrduavxk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxayupnc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvsfoliw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gujpemizd.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzszdcdm.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemqwezzv.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylnfijze.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gwprjzesc.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gmpmcokjc.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gmouttcje.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnalbzqo.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoosoerc.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/ghuqoysdf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gvtygbdae.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gomusxxhg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzclwfvjf.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gyuccgxvu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpzxxqvw.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gyorevkcb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjiciikn.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gjqeydtxb.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gesvmyzwg.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvquiumvl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnrsmwld.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdmqcciq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gasavcdag.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkzuwuwa.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelviqwao.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/ggtrnbqls.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsvwcndn.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gkikhracw.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gsjtjgpwm.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gdynedmlw.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/giooedtdj.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gzbhqoqlz.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gqfphhadh.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grramijtx.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmnzznbc.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/glmatrqxz.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gsekuwuyr.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gibckibjb.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gdnmcxknu.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuwxqxvs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/ggerckhed.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gvouhosps.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gbokeaziz.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpafilbt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gnovjmqmg.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gexrqcqdj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gqtrjtljd.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gvsztgtog.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gpfrsojvp.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gpshipnaq.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gitffkgql.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvxkydrv.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/geshcoadi.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqebqpcm.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gymghadhj.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gicypxstk.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpddkyhjc.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/goaqyqhyo.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gbjarevvw.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gejkuxjxt.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/grxluuzjc.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuouhxhe.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gbscgrynm.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcctrzky.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqmgmyws.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvpoousp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gldeuzjdz.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnczmfoj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiyqiugz.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/govjbsxho.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gaambisit.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gevuvaqam.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/galufzydu.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gabjtbhmp.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/grndzngzh.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyaostyh.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gvmbxyqaj.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gmbskbscy.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcqvzweo.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvpumogd.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gfltqgxzb.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gkdayhvff.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunjtuuyk.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gfddytych.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gerkcmjfd.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbbaqeci.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjrklkib.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/giottcffv.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gecpidhfl.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgmrauht.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggjzrtubj.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwonnzdlt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gikcdxqzx.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gditowxqe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goynkxdnn.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpdoqtww.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gjqvyzwob.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gixlrblpv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwgaostol.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grujrvwmr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/glxzjwlnm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghawwwfsj.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqwafclo.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gmgvhzktl.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwttbkha.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gbddnhrye.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gyectfirs.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqrosori.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofxujcwq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/goegefjbd.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwyzqttn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gztxyrqgr.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvvyhndl.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdlhfkta.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gvnjftaok.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdubjljb.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gljstxtee.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gahcqfkwn.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gooabricg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnyknezh.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwntsccg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gagntmorm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gthlvnjnk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/grzncadin.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gakbzhwmx.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gssapghcp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gtlblekcj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gwtqdsrzv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjohpdiwd.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gbvtebcbb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/giklzpgmo.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gpelleyoe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gbrtbahao.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgptaykg.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/geznjxvsf.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixhxiwpt.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gwimrrdjx.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/givtgwdlg.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneclcnnr.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gksfrsarz.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/geuvcbgfn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhxmrflc.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/grlitqllh.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhccjjjy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbccmdefg.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/geodivjdk.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkatnemus.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gfishvthc.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqthjxcph.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gdkfnsghz.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gdsvqxpun.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbmdzwde.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfcxdjnj.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszvjckix.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gaydaodyf.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gcouxewrl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gonfdfiol.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbavoduc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gicmddtgn.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjhytpek.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gzoxvjozo.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuyonaal.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrmzzyey.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gahodtosl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gepldlmpx.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/grociogtu.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxddmwyc.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gcggtxcxk.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfhzwnyg.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdnsuyxmw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/ginnyajhu.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/geegjopkm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnptxfpiu.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/ggschekby.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdlgnfel.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gyhosbwtk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gtggrjrew.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gjcgfshsj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gyykfjdyy.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gkikgxbga.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmomtaoks.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gywqlvxnm.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdsrfpgl.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gqhxzsqgj.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/glgiwfllm.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gpgpmzxxl.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggliqjzff.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gswfxsxky.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfdxdyfa.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsjnnwcv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gxqjaygcm.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmqvefeo.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/giymkgfdh.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gcpthvrhk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gemvpiaeg.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/ghojqyzsh.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/grxmfchys.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gyixuyorh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/glbuttkbl.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/guwplqljl.sHtML

Path(__file__).resolve().parent
来源：http://3g.fanxiaobao.xyz/Article/details/gquumblkn.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzellpujf.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuaarqza.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqgtsygc.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyshuasc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gtrgvcsls.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnixrfhq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkzbcriv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxdyhucx.sHtML


<!-- 参考信息 -->