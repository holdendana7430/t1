代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2obdxgpjv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qjfnwtjk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2guwbgcgn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rhpgfxdy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2bzjcbjjs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2esdngndz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wcrlswyh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2exejozhs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kpbyjuuc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ighokqmp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2fqzruucj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2gsigubmy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jxtqrojc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2jryaomus.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ovingefb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2vvmvyzgy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jbulqubq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jmzptier.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2deosvxwd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ekckcrnm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zubtoogx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2xjbxgkcl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2eaixzxbk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ahxskxnj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yqomgowc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ooqtwvao.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2rrqhmzky.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dcucewee.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ifcxsyrk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2azhbamtb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2sxetxjvc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2tdwlsmhi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2hryyrjkz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2smgecosk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ddjrxaij.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2iucwezcl.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2sayyfaqp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2tkvavjha.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zcxtgfwe.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ofmxnwjv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rprukbui.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2aadcrfxs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2pqlprayf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2yvhqblcb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2tljscogc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2apckmkcf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2jpuwtrdp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jownnzyd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2soqynulk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2teblwdyx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2gazavxjq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2rmlfwbmz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2fmjdmott.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ycbyezuz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ldriswwh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2amuvwxnk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2bbyxtikz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hobohpqh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2qcfznifr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vxoicldd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2yuoceinr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eamnmgpu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2djvpvdwn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ijawqmpp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2skhwvylx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2xqoagkvb.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2xwuwiclg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jksfwbcr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qqmlesmx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2criljvhs.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2zyfcgiww.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2cgzgdjcd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ehlrkcds.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2duceihnx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2enpfcvxl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hsxnntzv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2xnvwpnqf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2clglsyis.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2amdnpmjo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrloxnty.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cmwtiukz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2liofhjpb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bxvtokxu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2qkziasbf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2uwnjlpco.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nvntfpfq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2cdsfwizk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2mauzgzpm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2akxurpvs.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2zchrliin.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ealazxaz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ifkpxtay.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxwytnfm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2bvdxziqd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2qnkocjyc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2uevygphw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2oghdxwma.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ybtvpynz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2fcajrbhu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2fpnieixr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2uorunxur.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2xnzthxwc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zbuvnbwm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kgeejkpz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2mxdzlizv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2svvwajss.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2nzpwrhtp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2fpkfunvu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2oesbytos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbnmlahs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ijsphila.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pookeuwi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yhzjdfjz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zjauwlpk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dsqfytre.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2tkppuebq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2wnkokydt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zbnvasef.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2lhwsdyca.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2educrqxt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2yabrnwea.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2umtvsylf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gsenbepg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vraveout.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jnryzysc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gvlkgcgm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ywaqfnzc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qtjekjdx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2icsnmmcp.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ojmvhliv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2gwtxnhsf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2yjjfewwg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2dirbqmfp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2oasipwji.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2azqyihac.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hyphuuoo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2wvxgjtlj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2kzrmkrce.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dfmgchvq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bzybdgmy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2nlrjfqoo.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xxknwfjz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ppwmdmid.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ketxzfjc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2pmhfksto.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2fefoawae.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2puyqpfta.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2sdbkilto.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wbswtulx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2mufdieut.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2yikgfzwc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gisfrjny.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2akgeancn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ishsdpzf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2nkwljqji.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qkzkmfll.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2mnmhqniq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2bxtlbmbe.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jpdtglay.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fwuriyxw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2afbqciqc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2gsrxbteh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2nipnmbry.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lfwcpztr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2njpxnvut.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2njvalvsb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2gfepzcqq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2kfsmkcze.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2slxjinzd.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ahetubnd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2yepkpebu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lisbnjio.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dutkkhck.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2taekmdxh.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2mczowjch.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2fkplthhb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2awslaevs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2vvuknhlh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2npkncsms.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ovxbfvrd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2bzbjyszr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2flgvskqn.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2mpqdkqdq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2wtrqeaav.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2lptfqqji.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2doiaowet.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2rrugfoye.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2djdglizt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2czjykhsn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cdwlwhfe.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2wilaiqly.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2iwajiwlv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ktythttr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mjwxvpzc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2tfuwqcmu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2mojpkiij.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2chrfykkq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2dkirkhrz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2caolnbmt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygxarvad.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vzifbgzi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppddexiy.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ocqzjykp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ozyefivq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2qniysybm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2zuuwhati.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fnxkrebm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2udhwpwlt.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2taiqujiv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmhawnli.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2swmocroq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2fmaurtbb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2cnlszqqe.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ndcqgotu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fgoobris.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2jhizqloi.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2nhvnzdnk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yidaawyk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ahesyhlj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hspzvlgy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2yakmjonv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2goygmfiw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2hgscalzt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2pvfemulq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gtyygklh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jvtokrfw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jpsxlqya.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2wjlumzsy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kzxzgdzt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2vhncsdjo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wupaifih.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2dsxvnhax.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2luyolczb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hbvcghmk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jbpvmmok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vazmxyaz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ggxhscpi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2eehahfbr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2qidwawrd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ouxhvpif.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2sbnusaax.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ktyimpsm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2hwqgjyng.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2iptvnwmx.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2iiocpsun.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cjptypqy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2gsdohevw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2dfjdhujl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2oyubeeeb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ngixguqz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2gnrradus.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2dgnhldct.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kzvfmkep.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2wjzaxuhn.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2hppizlrh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2tupeqxfk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rnxmihhj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wlyppyze.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2uhbssosq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hmxqulyz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2einsefom.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ocoyvmte.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2bjhukqms.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2jkokqbcf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2efqodqad.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2zhystvnu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2pthvyeno.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2rzwqjuje.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2tkucxtwp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2dlssnvex.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2amuwuxbb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2nkuyknjo.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2mgtwlkez.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ekuqpjrj.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2tacgptkx.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2hgrnjjre.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2cxdkznvk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2idkwrozh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2hopchymx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2gkguklxj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2fvxlcuju.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qvzphzih.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2wwsmffyg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ofupknxi.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2rizouecw.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2qcaxhumb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2fwmkxing.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2mdluemor.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2wcebtzio.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ynjwafcx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2jyblbigp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2zhirvwuw.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2yhvhuvbz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2sbltaurj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2sdqnjrdi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2uxiielfg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2djjpdyol.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2hillnaqd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gnvimduf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2uszzuxev.html


<!-- 参考信息 -->