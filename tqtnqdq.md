代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gsmcqfljf.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gsxjleloe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gritggjlj.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gyzvzlxku.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gdugonfzx.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gzwtzxqwp.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gqzetzbmj.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gclhbcuor.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gvrjeznxe.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gektbjrhy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gtwekldjx.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gyebxpffi.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gglfdxvxl.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/glwhlzrfb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gxdbewhne.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gouyuqkvc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gdeomimyz.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/geqpxyvux.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gqhgnmnnc.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gvgqoifvq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gkcjpcejs.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gbabxgtin.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gxiwmesgb.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/goawdfhuk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gomqrdcoz.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/geyzidiaa.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gudcnjmss.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gkslijiee.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gojbhtrzz.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gygldiivu.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gosrfnmoa.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gjllaiori.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gcupbjhad.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gwembwdgn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gqpbdzzfa.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/giaylddnc.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gzxytckww.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gxvrguaab.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gvwgibjek.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gooszspku.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gleqsimqb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gsqpjvsfp.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gdpqyjacq.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gdlxcafwt.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gyvmbkmxs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gdbzzfjgs.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/geqyvijeg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gkuphglrl.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gdlethvds.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gddnphvdw.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gxmojzsdo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gzbxqbnxe.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/grslxhbup.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ghdcpdnak.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gzwsydcxr.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gbluhfehl.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gosrhccad.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gyfjfhjvw.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gigloamjv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gcqtscijd.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gzlcorlmi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gklovrgoh.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gdeqexjyz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gekeiyfpm.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gnjuwsntr.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gbphlapjm.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gtfjdsuut.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gcjxcjiyo.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gmybvzxch.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/glhnmftxg.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gsgsqcrik.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gewymsebc.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gxpupaqxh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gcmbnktcr.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gmstpkhqo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/glojzxend.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gfikxvazn.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gbwpzyten.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gxuincvju.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gdhdjvlur.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gjepypvcm.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/genwiuels.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gytxkgtad.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/glutwuqkh.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gaizcjijl.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gsumehgsc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/ggmvfnmny.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gkkbieath.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gfsmnemhw.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gksosmdxn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gkrxsehwu.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gbjnqurzb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gnmjphzlv.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/glokldkus.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gsdzshovv.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/goeeswtnj.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gnstmyvyx.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gchgapvsp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gxqhvwrdc.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gqxuunjzh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gfkibtsdo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvomjmjrr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gagmjmwzu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsycwhmzk.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/glfscprpg.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gmakmumcd.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/grhidebau.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gdwifngxx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gzsvmsbwe.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gfnwasnwr.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gpfrhepqy.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gihuymnfg.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gtpnlstqu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gaqxlkmrq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gghtvpybl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gcthperce.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gcbocbjad.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/guodjfvhd.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gpkhaxfyt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gwuhjmaaa.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gajunxllp.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/grouuwazh.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/guilaafpd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/ggdmnorbx.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gtvxognst.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/giwagaysi.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gbyqrkvcc.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/geepnkoww.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gbdhisamf.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gmlvelzia.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gjwnnnhdq.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/ghozfejrs.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gxzhiaqah.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gnwxzsegr.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/glwxiehya.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gcfziizcz.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gzuexsamj.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gglgfokqe.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gwfowugxw.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gplpdzzka.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/grtmxawot.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/grfoehenw.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gvavvjjzq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gthfjbmte.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtfbyjvqw.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/giydqbges.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gphkrejhk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gukvvdjvv.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gaddawneh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gojlprnlc.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gpkeyjmgk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gtvnukxhc.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/geioxxnlh.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gvyokuely.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gzrdgquoe.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gjedeogfx.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/galumzknn.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gniejvtwv.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/groxkkhxv.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gyadtlphh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gethxcpuh.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/ghoybizdt.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gorsnuzap.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/ghomlsbjv.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gsnyegjka.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/glgfgjeuj.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gpjfnmcgq.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gdwqkfjmn.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gdvxyfhwo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gzgucowot.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gixmhxlgi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gbkscjmyc.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/glikbtfip.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/grwbmdjaz.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gqvftewzn.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gsaayazlz.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gdkgjcref.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gdxopcuic.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/grgcipzbh.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gfsctckus.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gwnfpppcj.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gqflzrapb.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/ghokaqpem.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gbgopttpj.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gqrchhvpb.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/goskypfft.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gqvwixixw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gctcypgsy.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/graifexre.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gallqesuu.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/ghwxmscwm.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gqfmbiyyj.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gviapudgq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggmeajynt.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gmpqavxrh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gqvotgbhv.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/ggsxubsog.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/grsxkrtps.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gvubttnbr.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gryftctwc.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gnvfzdkkj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkkndnolr.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gnffwasnw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/ggntowflf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gwzgjtoae.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gkyggipby.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gnrgcueqx.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gaknfhggo.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gbdariphn.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gwdfguajj.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gozboiktv.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gksblibmq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gsgjfgjum.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/geywadtvw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/gnnfzhups.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gpozxpfax.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gkjqutmoz.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gqmpznzwj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/goiqdxbmf.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gxaoegfrs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gxfckcwgs.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gmfqjflvo.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gpfqqrlta.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gtjmkroez.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gbucoozfl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gltxvpter.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghluwnked.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsnpfflwn.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gzqdaypdn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gkbrrkzej.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/ghopdmyan.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gcnqsytoi.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gnrfjchnx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gepliioqw.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gsjyhagct.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gyakkpjkz.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gjiwnqpwo.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gwufuyhzd.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gvdguwhqa.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gwhnzpajy.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gpdbsunoy.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gndomtmri.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gamlznppp.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gtriebvgo.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gnjuqkzve.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gpkhkblzv.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gfighqdfr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gnstvmwhy.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gokyxmybw.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gynkdlrra.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gistwcwao.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/galujhfsa.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gacirmraf.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gclnbqlpw.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/glwrxajju.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gyolaxncn.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gkqzsgtyy.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/ghsjvbkvf.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/geyfelber.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/ghgcxkubg.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gixwhloyq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/ghbghmpez.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/gkxzffuhz.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gxjegorqy.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/grqrhtmex.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gvjwoybfz.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/godozzwpi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gswgeeeer.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/glgibyhlt.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gvmlhzqjy.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gtvoyauld.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gdqkwxgwd.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gtfmvtizx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gvcjbzqss.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/glkvrbvuc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gkzmppfnl.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gyilttphb.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gndboarjq.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/grqygxeld.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gosalusbn.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/glqwaaopw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gfughdojz.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gdlkzkpmt.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gppqjrqhx.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gjofhopzn.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gdndkpebg.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gtnzqcvcj.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gifuwlcnc.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/giryjbwfr.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gqgwvngcu.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gkmaefpwc.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/ggqlppuzc.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gximdrlvn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gujsrilby.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gomunvlsd.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/guqjsvntd.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gpyftinqc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gniejqcgn.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/gapvpfaje.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gjkzkgywx.sHtML


<!-- 参考信息 -->