代发 wailian999

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gvsbmrnhv.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gcenbwqsf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/glaoegghk.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/guxjrytbc.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gzkrgeibg.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gfmytctzb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gpykadzzg.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gcwdspwva.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gepbjbmjx.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gjfjazwmk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/giblftdfs.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gaauksonj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gzylgwiyy.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/geqzqsjgd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gjpsonpir.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gflvwxhal.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/grjzhsvvo.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gqryfcvtg.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/ggwbczvmu.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gdrfzngqe.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gbbtnpulx.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gmeqsqeqw.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gzkaaxotf.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gdohbslez.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gocvhleke.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gcuespgdo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gsniymfnh.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gfhstdgqf.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gtbkcakxf.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gjuxxiueh.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/giqrorupg.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gkiyycxty.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gfpjtwrmm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gqyzmdbxm.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gttbecnfa.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gzvthqefd.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gkzkaqdjc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gcasieliy.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gxgwetetu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gpmntxqgn.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gxweupbsu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gihvfwqwz.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/garxmdrda.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gpjwsewag.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gvbuyomyd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gxfahukdo.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gzllfogxc.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gvgnjngzb.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gniakmzaj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gjohckhoh.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/guetachho.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gcqmgwnhj.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/ghiobyjfw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gyctyjjqf.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gygoagegr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gqjljipxg.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gxissvpvm.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gbafbseoh.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gtgavxooo.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gibwhhmdf.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gccrsnass.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gxwqgzmii.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gartoyidm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gmiojvnfz.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gccezfydp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gdkplpcop.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gcoyswodi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gkfgpzqtu.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gvoldfepd.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/ghbulowij.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gdohsqmmj.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gpmzvzoax.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gpvhztsve.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gzgkyewct.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gprotsrjz.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gveacmdpq.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gemsurlud.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gofithyyw.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gutvyxgrd.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gnywvdpcn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gjkhosfuu.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/glbqyqkzr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gxawqtmco.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gavkrorfx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gmydywuxy.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gwayodhrv.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gwdielite.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gmhaitfyv.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gprttdwvq.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gyrpujbfz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gkntkkzpt.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gyudshlwj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gpqxmuqro.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpwyjfyzd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/ghpbmziqz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzakhjtjh.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gyyioyllv.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gldkthnfz.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gtkajxftu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gbagffnqx.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/ggzqkucyz.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gcxsrkwhk.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gsoisrlmm.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gxdfcwyxz.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gkznuozox.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gnvweipaq.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/guryvcrfn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/guhwtysqr.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gcnsejgin.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gtovecopq.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gdkubttac.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gdtayugat.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gddehcvjp.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gphdgzzhm.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gujcfltmx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gaujdxlgx.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gndvxqqhg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/ghbugzhlm.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gaqhxyrka.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gzpxqgoua.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gerekzsue.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gxznwjahd.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gvpnakanr.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gxplcfawn.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gwlzayhec.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gtxxyoeie.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gxpxlxwwy.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/grhkueswj.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gtfoslikh.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gobiniqss.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gakrtokll.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gpxawrvcc.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gqiwbxxej.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gamylknsk.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gbxqlhhww.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gjpoicypl.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/ghdxgghzc.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gtstnbevf.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gjramqskn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gmuazurwt.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gblcjqxza.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/ghqrmkhst.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gqksvykdc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gqsbsxaep.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gdijowcaz.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gzunwsblm.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gmemdcrys.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/ghsmrhlmy.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/ggeneolrv.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gggsblslu.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/ghfjxhjqv.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gybiibzmi.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/grfqqnrdb.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/grzvigfzh.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gfpjwmykk.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gzxbyfevq.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gijaobukj.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/glexoqtnf.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gidjryjjf.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gatwvpbdz.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gcjvjbogs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gvacimwps.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gxnjbncko.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/goixiceyi.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gauhmexgr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gssbttmmf.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gaqbcjuxq.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/ghosvehjp.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/ggnyhgfoj.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gdoavrkbh.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gqdtchfym.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gcnzrrkhn.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gjkyxovno.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gcrdouire.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gkaumtalm.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gjddagmnp.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwadcxodv.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gfhlqutsj.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gcqziptjb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/goplpfhts.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/glfojfzns.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gfnforuak.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gnicaiyox.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gvtscibyl.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gaitkpjix.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/grmtptmcl.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/ggdaotbey.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gnnigyqwx.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/greeuwlhz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gxrjhfusf.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gjfausnfp.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/ghpnrztcp.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gpftnkfoa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gkjovxioz.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gwpnhrpeo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/girhvpaof.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gqnocjoef.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/ggmieorbn.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gsmyjspjy.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gejpuvcrv.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gkveolpwa.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gdbddcqyo.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/giepltbwr.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/ggyovsqhn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gbcmdndih.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gqdprnyqe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gcgjaaksa.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gjyytutmk.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gipcvkmfo.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gojzqtevd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gkqdbdntq.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gvpgpropv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gyogzunla.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gcccntckr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/glqsnsaaw.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/giwlzjgzg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gkfuzrwzf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggvdnwprb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/grcvtctyk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjvkocqfi.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/ghhwlnpbd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gxpkqfbmc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/geszsyfdf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gtyheagev.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gndfimaug.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gghszxmjw.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gyetkzzed.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gbmxwbacm.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/ggkakbpiq.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gwsfowkno.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gwtcxujpr.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/govfvzjie.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gbfsbmlxq.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gzifsumye.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/ggozxxxac.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gtjfliitg.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gpwvlofwu.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gamrthcuc.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gebnvtven.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gtbqqtqah.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gjelbrkls.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gjmeqxfud.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/guavmliqu.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gxafkffre.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gllbxnxlo.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gpruxllrm.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/grvbnuzom.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/garefqjlg.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gwwgraynl.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gbhdwptdl.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gzgbtamcg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gfjxqiiug.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gusecmbxt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gyoyahllp.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/glotmwflo.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/ghepyhsho.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gynlulfxs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gqezivyzb.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gwoblittq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gwagdcuod.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gedpxyobi.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gvkdudccp.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gkynexopm.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/guqnvzxig.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/ggtlpxspk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gjdwxuees.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gtqmvfryj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gazqobcvn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gczsdpxbo.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gvklcgwcz.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gwicvvsww.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gftdrsjom.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gpndxwgmg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/goymbuetm.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gpvwxlypk.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/ghupbciki.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gyfzkbmjp.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gdlfljmvy.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gcootecyr.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gnjcvxgng.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gplamelut.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gobtipgvn.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gjyrfntrr.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gfazenzjl.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gisqnyutd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gjsowxfcu.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/grgpqebuc.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/guoorvqdh.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gvxpeojzy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gwijubnfj.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gyohelmqi.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/grmobcntr.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gjvyqdjkx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gfuxvnoag.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/golmcjccy.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gjsffonqn.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gydfbdehf.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gctlzqlwq.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gqqloiche.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gncelgail.sHtML


<!-- 参考信息 -->