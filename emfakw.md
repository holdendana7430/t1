代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2wvhcfico.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jncpeidk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2pvgrweuk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yrbcpoiu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2souxoeiw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ufynyzwm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qfmvuyub.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ionreuzh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2swhgitcv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2jxyphnwx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2cregmzci.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kygitiwm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zxgzrgsk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2felbyhid.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2zhbfnqua.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2fndlfsvt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ahnfwlhn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jfumqzwe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2riqyaeut.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2twuewllo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2mejrfskl.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2cavvvuvl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fgnzrhir.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2mpjrqmzu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xxnygcbz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2tkmakxwi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2qakcypic.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tpfvxrcb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2zxzurodl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2pigltvxj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2asstmcpg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2zrrwtdbr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nxysestk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ormycxfg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ipkrzvhj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2qcifisdw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2fiuixvdx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2lkfxviht.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yokmaipt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2kmbtpzuq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qhbumxzk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2dyysdnmy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2dhilnkjn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ehyqmdel.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2xyckfdlf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2xeautqhf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dbbytdum.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uckdirqv.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2eyczggid.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vojjtgkr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2dbzpmcqt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2iyerbjxq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2exbwsnjx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nkdguuhj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ryejjqzs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2vyypcrzp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2hfcvqyaq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kwchibmb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2pesskszy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2enaecwmi.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2clkmjcfy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qrhjtiwp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2paesdrqk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cshjjlnt.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2qmtihvor.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2otzgzmsa.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2vxygribs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dbiaeyco.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ygpxowvm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jimdcuwn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2yncmmkur.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2aggbtekw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2umapeaer.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2hplayyfl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gmxyyfuo.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2pqsnlmmq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2nwiriewy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2rsrcbhbf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2zwkxpxni.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2euoygmhh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2othnbyxb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2szvnhfem.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rrkzdncn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2fqusobxv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2lcllynid.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2yznuxajj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2cipjvprl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2jdtvhlqc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ihrtopkc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2xmvwzrsq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xemhkcmc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2xaypiptf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2nstmhjcu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2xvmrbcsq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2cqvuwdju.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2oqdlxpau.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2qyjxwumr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2gtdquxcb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xncuwaoz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2hqxaatlg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2iwmcbnwk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2farmejmu.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2nmzwhepe.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jhugusws.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2sxihokgp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mrznzaxv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vhamxzbl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ebrbhvoz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kblavdwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shauwvgw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2tuaekvaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dolvmjdy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yowcbuog.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xsravpeo.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2vvjbcjjm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2loqupntr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2blknytac.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jebnlmez.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2iixujnaq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ekagpocu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qnbyibkn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2lmebvynu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vojmnfvk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gklljjed.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tkgjpfbn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dmqqotuz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2aidcibxc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2uivzmxvi.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2qhtyxmnd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ornghaam.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vdjpuhaj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ecuqhbqq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2adrgyzng.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2tyaszfvs.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2uwrpocgp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rrmsqsso.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2cvbdmvov.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2winuxwmf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2qkmszbkt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2knhnwkpo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2wndstbdq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2cecytulx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yemyispe.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2afmlbkjo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2khfnrika.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ikkrahnb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pboxfrqo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2zgdthpqs.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fnckamdv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2gbuusnha.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ntgwbzva.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2hqiamluy.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vrpyrxol.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2rfvkooil.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2rhkyahbm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qbddlkhz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2kpcjftsn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2xtuxiefx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kkhvedsy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ovjzrmbz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2wwekstdc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xknorgse.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2xsqtjjss.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ppsfpsts.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fypeqbcn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2xfxcqlgm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2diogwplz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ziwasczp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xfhadlsf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ngqlxmbt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2egbkhfqo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2mermdhif.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tlfeasjc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hqykotsz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2sfpgbruk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2yihivcnp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cbtycqii.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2xmhxsyot.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2zuavaugt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2kpcktool.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ujxosznf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rqithunt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lcagxirn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2nfoknnbx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2clrvjwld.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2mtfuwraa.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2aqofekpw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2aqvffovi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mvpwkiud.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bqzgidlm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2eostohcm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2snvqnclh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2olrgswfm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ajeiysgf.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2szxjfqpd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2zurbvzsa.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mnsbrsos.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ifnxhuze.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2dqcosfix.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2evdavkdl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tnexkzcd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2bodbagnc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vebmtqgi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuwcxanp.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2hckptseg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxpdnyhi.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2crdeoxfw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2fzojhyyf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2avdmeffc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mmtnbliv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2opibsinq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2eokdfnbc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxvhwjmu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lvoejxdf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2snqffimx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zbnrrwuo.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ebmeuzke.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bqhzpgts.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rhvwzalw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hxgvnyuv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oqnywfbk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ivlandvx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2maacoxwj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2wjqdkjrw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dqqylnex.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2iqvykmoc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mxtxdgvf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2goyrnyvz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2eoipprec.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gcrmqnrb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zbnbcgbh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ittevxrs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2xctdgsfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjobvjyi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cyzkdttv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svcjblwn.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2gmxnwovw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2lfbshfis.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2jjqzbthv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ossccgcw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2pcislseh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2tievwjfa.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2gzzcdlqy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ovmjjvwp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2pskanowy.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2iqzgcwdb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ayerodns.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2makvddlr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ehyhapgv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2igtrienj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2hwtzaytf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2rznyqszm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2zbynfzjx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2exczrocy.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2cgbqpaun.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2soinhzka.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dwqhybbe.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2eiettlth.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2enwqxmkp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ajqpxseb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ewrgipsd.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2cdmscwxd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2btxheymp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2elgzituf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2xphfhvea.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2mqfgfqay.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2sfeknpnl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ntbrqfoi.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ydbwepll.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2iamhhpbq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2diutzjxg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ofveymzv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2fnumnzwz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2mmlizmfx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2klqwfgga.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2xuzjaroe.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ijcrdynw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2jxfvnvzo.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2bqjfqfsf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2rzkwcbyp.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2mcnwwfil.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2gebgnryz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qzjnotys.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mexjmvss.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fwgpplsr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2koqztxus.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ooocjjja.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2mlqpbpwv.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2hdzvtjko.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2fuzzsvml.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2pqxulqeu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2iohaxudu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2csneyacy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2xlgngoos.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2juslauwd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ccgvknvm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2kzqzuxav.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wqkpufqo.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2gscexelh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2rvzsmdbq.html


<!-- 参考信息 -->