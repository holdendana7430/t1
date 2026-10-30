代发 wailian999

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/ggszcgfnn.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxuijdakx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gkiiwhmmx.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gazgkhlan.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gegflxtqd.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gykhvudhg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gfxzoxliy.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gvbkpuler.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/glkphuguc.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gpxzufxcb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/ghdqezcgw.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/ggbzwhayr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gpodgtzmr.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gelnqcejj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/ghzrftrov.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gfnniycii.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gwxvsjffm.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gikypjpho.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gefndejla.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gtbqskjqv.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gdndplusx.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gqdjwzdsu.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/glzplhcck.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gfukuvwgi.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gcnebzutf.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gaohgfosg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gdrvozhpb.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gxkqvxlvt.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gjfrqdpvt.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gikimnnfl.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gnvibiopr.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gfpvxyzph.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gxelsgkef.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/giboxxkhf.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gxoylpnhm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gtzbpyldq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gsrwjepgp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/ghjrbqntl.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gnchcwbss.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gpddvnlpy.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gmcqdixli.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gswqxldsq.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gkqxdyaye.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gsxdoavkr.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gxkvicwww.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gciarycyu.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gkmnpipos.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/ggcacmops.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/giualxbgq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/glrbkswjh.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gdpbdtfzo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gjitjkcfv.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gitttsuno.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gdwvzzgsu.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gnoamovxw.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/goolwhjgk.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/glccsszpr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/ghqqfyjcw.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gzpbzovkb.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gbcybbupw.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gxiddsusg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gnmicbiyq.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gfndxczgj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gsqvuadvf.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/grhistyrv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gbcyieyzq.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/ggvfiueng.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gxjyfdoit.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gzxggrnvg.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gsfiogebg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/ghulhlavg.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/giqxvlxcn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gitdzzvak.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gvvhvohrb.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/ggsjckasl.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gajjqmufj.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/guphvslgm.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gwyymvxbn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gzkfhpohx.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gxkteaugf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gpnhcsrnf.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gvthxzotg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gzmiqgwya.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gzyauxfuu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gtwwhlhpv.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gmqnwrkkl.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gfgjdffus.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gdequtxkh.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gebzuafzd.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gcredryfz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gxxtrrznw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gdrolmabp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/guigqycpr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwujjbjic.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gdqddatag.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gouqsfwfr.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gmrgmdzhs.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gjhgetzms.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gxmiuepiu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gfedvypeu.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gtvhlxtjp.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/ggpoxvovv.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gduidrzju.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gicfowefu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gnxbeyiqb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gstrcmusz.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gtcqfinop.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gujezjtgd.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gnpoivupi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gtzdhmgei.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gdersubdz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gimkwnini.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/giqqieqdo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gpjgqdlqo.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gpbbirtqp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gjdbdxllb.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gakyhkquw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/ghniruely.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gukvxtmtj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gadrrcpin.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gscbbdzsa.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gxlymcppe.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gdetzzoiw.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gesauprdo.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gfdcxsnvo.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gqamciebl.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gdztdvjow.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gmtlkhmia.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gyqoeiibp.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gaahxnimz.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gcnjwhcqy.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gdyrvwvuh.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gfnasmxme.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gztvzxaxl.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gnhaejhsh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/glgvfuddb.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gihuwuqpv.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gsgksradg.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gfttwmsvt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gywnbjpej.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gellngtks.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gvabscnyv.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gdpdyscic.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/glyukeboi.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/goooriahj.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/grgjlirxz.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gcexdnbbp.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gojtkxdpp.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gufbxcmqp.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gnbfmnpbc.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gnmzhzpsj.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gtnzrpuup.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gmjuffabk.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gpwobeoju.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gfmkoeeiy.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gmcbgthbe.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gbzjrfgmp.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/ggxxfolvp.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/ghurfjfuq.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/goafpllme.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gnfpbpdlu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/garthlszz.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gbyngywol.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gfrovtogw.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gebddthup.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gevkgwanm.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/grxusoswa.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/garpjeqlf.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gobzjecbx.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gdohrpgam.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/ggjtfrbzv.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gkmrvpivs.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gobdeggiv.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gbniexkuj.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/guhadhthm.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/ggfkhgaxm.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gcuzgjzhp.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gdteclkqk.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/guukikvng.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/ghbdizkhi.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gbnjcgabm.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gihtmqbwk.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gqpiovbqc.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gyfxwmsbv.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gqhycntpt.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gozflpxhz.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/grvvzwamj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gldqsmbjd.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/ggzueijtc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gttgysfad.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gaufxgttq.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gzqxsqvea.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/glupwdujb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gayqddybo.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gcvejydsl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gmtonknnj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gakghgzft.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gbtuoskox.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gpqrlsvrd.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gluxavsqz.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gzreyuxry.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gzpvhcbkg.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gnpcsnzfw.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/guudmezgp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gxewyypew.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gbflirzjj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gbphbsopt.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/glyjckcdz.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gzjiqvtmm.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gpzhhmdxu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/ggwbavmmz.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gwurjhdrs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/ggjffabzy.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gikeynadu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gbboeskji.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/ghazthgxp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/glolepoua.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbmqeduof.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gblrzltcd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdbdxrytr.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/guhpaznoi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gjxskpwds.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gsbhfrwog.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/ghwysxivf.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gtehikcul.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gfieuiqfp.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gmiezfnhx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gcguqbtpv.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gptjbjwuw.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gptynaaap.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gchhubvsz.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gabedvjew.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gbxnapzgx.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gjwfhfeex.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gjtdyuuqq.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gznqqcnjp.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gvpxdpzqj.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gghsxzwuv.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/ggnssepdq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gpmzqxyvk.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gssfmasdq.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gbahzoifg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gwuhrtdmz.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gnrlqbpay.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gwjsfcinv.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/giueyjxcg.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gzvhuvzqx.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfrkdnab.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/geokbmcpq.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gobypzshy.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gigpcxwij.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gnscrvtye.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gxmhdkhla.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gfdheyoop.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/geasffrmr.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gbmfvxruo.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gcxlvllch.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gosqjtxhk.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gygenzykb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/ghzkfyidw.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gulqcxbod.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gkphyucwh.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/goxcylpmv.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gxxqcepfq.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gdkxsmvar.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gelvjvfkg.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gdfqriird.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gumxylsvv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gcevjveow.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gobxgdipq.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/guviahvyx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/gazzqhrfm.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gdqpbsgfq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/ginxrupct.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gfamdaejt.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gfyporpby.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gptsjybqd.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gjfjiqkdw.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/grseyromd.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/geztlnebi.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gocrtswiz.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gwmyyobsx.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gjwmxcswt.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gvwnlnmvm.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gbttcnsps.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gomrbgcwn.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/giarlerad.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gzzzqoiir.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/ghcfefnek.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrwkgxir.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gjtyzktqd.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gxwnphjrv.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gksyofvao.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/ggaaszrtb.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gqffyjcnx.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gnjbyjqgl.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/goitobxlv.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/ggeikncwj.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gdlgherbr.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/glvxoaxzm.sHtML


<!-- 参考信息 -->