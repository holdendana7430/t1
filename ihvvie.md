代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ejcrtbkm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3agxqtzaz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cymnbvlv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ognqzaak.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3iujkgzke.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uehujppe.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3aaoyqpee.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ryvoggis.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3htmvllys.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3wogxeyds.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3lfkygtoi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bwsystdb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3gmkbgnaf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3gyicmebw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3plobskyx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3nmvfaqzu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lunjazni.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gqglggjv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3pegfuhbb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3axzoxxqh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3fmgezvmk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3jokwxbgx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3otvdhpsr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wpgxabte.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pxcwyqjc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3kxmelngf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3wzkptvdz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mnhouhth.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ltuyomks.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qbdofkha.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3yilonitu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3fxmlpzax.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3exioenwn.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3vbprswos.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ifbmsxfo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3bvfiqayz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3smklfdnc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jzoufivc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3phwrfbaa.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3qorciunf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mqlpqmpv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3kmyplhxg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rvdotdes.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3xnlszinr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3fohpatad.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3riszgcya.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3souzjcyx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vtusdfes.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ciynsnzf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyrdcuzu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3uqscpdew.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3dmlhovat.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3qdbbvjju.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3kliacjfv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3rntkuzuw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcyafgmw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3gjhzwgbt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jxxextul.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3zebtlqje.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xpsqokdp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ycquieci.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3udkamnvq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3jgsjesaa.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3aqzqikvr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3denlszpu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3xempfwys.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wslhyfnp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3govbzrnj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ujnbggcc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3mwsmegss.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3reefgclb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3mukvvzyo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bbxbfrju.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3aalylkgg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3jvtqdtpe.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojumfpqp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3htfweuld.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ezmotwrm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3naaigzws.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ambcuhzb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ibtvesbs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3dapozmbx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3idedojmd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3gqvlspbf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3jayylhvs.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3liznwndf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dvqqrjcx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3hxsvqehb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eheykzug.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jqlclsof.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3jbccqqqc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jjowstgs.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3imncitgg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3dwztjhfy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3jpzyjloy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ofivdttd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dscinxje.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nxdgaftd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xlhulbha.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3pixspewk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hnyqvacf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3wnudnpnm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3qwqcebos.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3gyynotwy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hsofgegn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3hauaddhd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3hnpquest.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bpuwqnko.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cfwnmuyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hesobbfz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zehoixwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szihsocb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tvmvhyug.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vetgwkok.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3oakwxass.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3dlpcxvgp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3xgmucesa.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ecqluzmw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3gvefbjyf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3izflxxvk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ykgrpmac.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3oqtqgdea.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wrnxscrg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3droxqtfy.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mqcszvbm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ekydwvwm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3xjiqgxwa.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3oskchong.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3plkusovm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3heitbuxh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3zmqzzazn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3koqxtolx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3flucrvux.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3nygruugb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3nizavzhl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jbrzxxdg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3kvijykwl.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3oowqaqqb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3relahemd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3olmgkqls.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3mwtnpzgq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kowusvku.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mhybkcdr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ljlzokzo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3vatxkeso.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wghhvmiq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kodvjzet.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3rtvqlype.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rxcyucck.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hryhtzpc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3srnatkiw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ddecjfqx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ighorkbl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3pupwmukh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3miphgigx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3xqkusjln.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xcfdwuql.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3jafkaoyi.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3hemqxvun.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uxmasfvc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3mhuxgorn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3xebgclmm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3qbmzvuut.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3kmxxzlfh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3pmphrqcq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3xxpkzzoc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3oobaczma.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3orxrplbr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3rwkjfnnt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ehzfhkmw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3idutmccy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3svfzkoat.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mhwhpzkx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tpanebty.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wuxcajlw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3aapwyjlb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zzsjxeza.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3czzfcold.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3croufjrg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3cdjsndjo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3rmtvktdc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fadmcera.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3hvajgtnp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3lqabdcru.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xetbrjcc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3gcexsujh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vkltaqil.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3oavhmtdg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rmkuqilv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rqrjbtnn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3qaqughts.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3vycoonip.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zdgvdfxk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3toqiclka.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hrdtbhxi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3pzcxqxgj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eeqdbnbe.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3jfgpymxl.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3lwckcixr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvjlueiv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3rbcyybdw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3aywvrgzw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3jlrttgtx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtmfumen.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3wigrctcu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3soqggxmy.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3mnxqkkda.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3kxxkcqsf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hggbidmt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzqoktkj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jzxkbyrh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3dgrltqlz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3odvafhwo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xnrrwdzc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zmzevzba.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zzdpqear.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yiiflfkg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vjbffsbw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fwuajlcu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ziejihzm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sabxyrhs.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bslzwdsh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3cfoiljad.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3pnclpflp.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wadqywgu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xlqybnzc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zrsdpvpw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3xhzxgpvo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3dftsfxvj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3enjgddxo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ahsjlush.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3amqwvkmf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3zastwkje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ioypfgsa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3yfcisjyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzrugtpu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3jcceumiz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3liumybpk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3hphcmeha.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dqekttce.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3liuhgvzz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3kepdhetw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3jylymbjx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3wpshstvl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3xfgfwzab.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3kqjnzjpx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3cmzpfhnr.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3zpezsrey.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3xdfydkan.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3rdjsuhde.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3hvhqxlln.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3whqjyevi.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3fmjmhahf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3usqdvxdc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3kiqabuth.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ymlsmbah.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3obhyudbu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3bjmlpdkb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3gfuwdbvf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oatmdydv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3cxbwtjaa.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3bubiyjjc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3lzratvqw.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3heefbjwp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3qgjrcxnf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3rnxvskcu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wdfvsmdb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3efuecnbc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3kysbssek.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3egvdqybb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3hvnybbkq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3bzmixkto.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3azvcrhaw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3jebopynr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3awuvonhr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3vhtyaive.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3dvbxikbi.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3woaposvh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3csdehrze.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3dmhyxklf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3pvhukiri.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zhypnmno.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ctqqjnas.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wcbtttws.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3zrlqzrvq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3qyvhxcea.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3vzmezuyc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3epyfmnfn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3hvxdjowg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3tyduwnog.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3fjgqoncr.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ujxulzif.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3agcvelud.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3yrfpymcd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3efuuxoes.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pameqafb.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3zqakisev.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3smnxyuwj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ndczvvqz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3qhlfljec.html


<!-- 参考信息 -->