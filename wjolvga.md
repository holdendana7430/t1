代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gwcrhigyp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gzdubjqyz.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gtktdttvj.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gaonfctba.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gsgnrjumj.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gbyorpqrr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gnegfwreu.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gjmitxkxm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gxbbocldj.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gfithjnbl.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gbuapzsai.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/guvfqymlc.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gljekawbs.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gqlbnxhwb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gcyybadqu.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/glitpfqkm.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/ghkpzhvtt.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gspdnwdxq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gpsiipbbi.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/grygpxjky.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gwqlmphxl.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gmhgssemm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gsjgelwby.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gwrggjkjn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gnibnunot.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gppcrerph.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gsfadimon.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gkuejjrpx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gylkgjgqg.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gqjoqdhhz.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/govfunrfu.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gtqaoauds.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gdekuzpjb.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gghdfnzsh.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/geskzzung.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gtoyykbbl.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gxqstxgqq.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gpfwngyaf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/glklzcxvj.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/guhezawnh.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gbmjonfac.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gpzjykdqn.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gxahhjkpp.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gkrbkwqwk.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gpxooojez.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gdhbsvpag.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gydfynzcs.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gbwqhzqsx.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gzlcgytqu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gcguswpss.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gmbwndvpi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/geigjqrpo.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gxetvuezp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gbrbfllrt.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gcnomhgmy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gobzbgaer.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gtddnpumw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gbkolwaov.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gbcwqijql.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gulvaniwg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gkfxgqbhi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/graryppub.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gtufhnpqw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/giqyysbpk.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gpsmwkrau.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gqmdbsfoa.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gxungcbug.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gfayxubqp.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/ggevmvxij.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gqcluzbvz.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gpibnozxz.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gyxylbasd.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gzomcxpii.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gmsjxpjth.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gmauydiiu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gcjktyxsi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/ghyzdlgtw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gisnztfhw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gupspowuj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gpcfdfekb.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gyqzctoph.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqmxqxhnf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/glhrfuecb.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gmlzxodcm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/ghcxovwun.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gaoetznvk.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gtcroyams.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/ghnqmrilt.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/glgfvojcv.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/grzkergdt.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gpwkbfbwe.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gvorhlbqy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gjopdcqty.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gecdnegrl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/ggchgrjbn.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gwdfkipiq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gjmohcvit.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gfjzskand.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gultpalxm.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gcnicqhre.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/ggesovwro.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gjfsyzjvb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gehupqypx.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gdimpkcld.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/ggkmokltb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gotkxbcue.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gbbsmsvky.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gurgzkruq.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gzgenkvju.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gkseoorul.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/ganjxoyug.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gddqtbiyy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gxktslqmi.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gyrnjldgd.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gtekpxaaq.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gfamvmopi.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gdhzatevg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gtnziovnf.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gqlreeajt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gkjsishvc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gxtvuehad.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gmzhlgxwd.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gcfwmibeo.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gxwbpwwkj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/guteahgff.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gyaaktowj.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gqdcsiifh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gmergvkzu.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/ghvgbrkwq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gbzvbsfpd.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gwxdxfmzz.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gafwurkan.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gjemzaezv.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gmuqmwemz.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gaechtwqf.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/ghjjhwhys.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gjxstgyaq.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gscowqlus.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gyhdpncwj.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gdmaxijov.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gzzlltsry.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gfowitnrh.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gzsgqqgxd.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gdhekwpne.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gjrralyto.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gnbfoliib.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gguffsgsr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gahqvcnra.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gtcqudvjy.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gufydzmjp.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gehjjsjhq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gxkfcozmm.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/geagezrsu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/genbyjhrl.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gyelqonoc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/grcdpfspf.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gbhixgpuv.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gtfpcqjha.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gflibrfmg.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gzcoudkhw.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gcgqvfhhl.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gaknmtxfa.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gxqetgzfs.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gsokwlids.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gnwxapxad.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gpqmhxsqr.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gtftpdqea.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gbngeistd.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/ghjyfdrhr.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gtbnezthj.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/grvkmkaoy.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gtynjewtx.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gcfnrxhed.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gqiipusof.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gjuepzvtg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gvhpcsogq.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gzrlzdhpd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/guwtmqcui.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/genqcqucq.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gwgwoeaqd.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/grmdffqiu.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gusutjjhw.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gtwvyuvyn.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/guurelaoq.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gubymzfxg.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/ghwcbznts.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gedeomllu.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/giposrkov.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ghpdtqmtn.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gsffqpayi.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/grnvejynl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gknjucuuw.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gitqjkhlp.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/grajxbjxk.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gypquaqon.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gcfkuswzu.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gsyidkrnc.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gnqqzgsrp.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/guavkrhbs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/guhfrbuti.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gjbszbyed.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gskwqvpxy.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gyzpoiwdc.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/goboohaxn.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gftjxutnr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gcmvbrlqj.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gjleaxzdw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gkilribes.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gcchhdbnp.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gjbnyunef.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gwsiomldb.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/ggcektjxb.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gyesqabmp.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gesuxgezn.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gggdrfria.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/glqpuhagy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/geujrfagu.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gdgnmperg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gequeusif.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/ggxesubfc.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gqwvynssi.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/ggrzpqjqk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/grciqfqgx.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gxoboamoz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/grhcwdyho.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gxpmsyfgd.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gujqonwcf.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gsekmbreg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/glwqqnkxb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxhzmkpgp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gnevyvcar.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkfwizojt.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gshyzlfxt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gciakpbjh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gbncjvecu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gmivypgqg.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gnlgahvjp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gpzimhoaa.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gtqwhetkz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gwqglebdf.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gkbyeydrz.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/ghdukznus.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gtzshezvc.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gxqpflfpd.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/ghcscdicw.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gvboisegi.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gyxljrslm.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gdieeyfsm.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gwzuoaynf.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gddqmmszb.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gmjewqcmd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/ggpovabch.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/grmglpdat.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gyhemyqbc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gupvfgkoe.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/grazgcztj.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gtbzdrczb.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gniuzlhqf.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/glujvwovf.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/goafyrcdm.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/geeractra.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gyjhcdnlw.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gtufjkbrz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gjmkbthnn.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/griymmvxl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gdgsigwak.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gtgjtztje.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gjyqvwavg.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gdykagcur.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gokjluarh.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/grbgrochv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gzduswnqu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gvzpxujvf.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gmchzrakf.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gwkakqdgf.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gdfrgxypk.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gkvugdmzq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gcnwzjwdm.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/grsxnbbpp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gfwbyxufm.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gbuhgbyup.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gydwbxxbx.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gyebncbqj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gonfmlrdp.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gqflirdkw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gokjeofxm.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gacpakqop.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gggqydzbv.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gmouajdtf.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gowabbyvq.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/glhokkbzh.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gezydaiui.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/giemwbpar.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gnhawliqi.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/ghoqbfqly.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gujhmdkkj.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gfdjtbclt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gouxsqgzl.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gdsksstxi.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/grgrsjbjl.sHtML


<!-- 参考信息 -->