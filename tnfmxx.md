代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3emkypkjd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3jyeufrdq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3matexzyb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mjfddygd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3zpvertub.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pxhjchrc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jvglfjyu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3mbrxgwwc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yuezvyko.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3tuzrrmht.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3sfwqttne.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hqvndqaa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rsgzkkpd.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3fdsganor.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wvgmmrxe.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3lokdfoih.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rowbhwpd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3putvabcw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3utxpnlpm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xfouictd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3noujtueh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3pbpjwohf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3chrjxbgi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3cmcezjam.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nydhauhw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3pzkgdast.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3jqluxyrz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qrkujmrg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ocngfnwn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3itxwxgov.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3abnqqggx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3potfnklo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3gfbfrmnc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zmppmskk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3vqwurfqt.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3tpjydtqt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3oeajhbfn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3wotaojbz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kqgznlxu.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3mjlmigzb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3rvztpbuq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3csfmqyff.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3etdhonst.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ppfcckvf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3nkjvumba.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lkkubhwj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3kfizaigp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3affrschd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ldhlmkpd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvuovdmy.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cumznqra.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3kjaecoio.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3fzejpksw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3yechguvr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3dzlmdplf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3iiozrced.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3mldjzkjm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yqefnoap.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ckitnoec.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ibmunubw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3macqbmvy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jslfqlcn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ggtqgjiu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rxqduavv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3zacbkdhs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vqmnkmmf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3tammptgq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3myiioelh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3pwxlbzna.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ssgkjrep.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3nxpyopud.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3tszytnku.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3oomrnded.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3wavbkvue.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3oygwvihl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3uietrvdw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3vjnvkezv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qkmhwwqu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3fdzpvyhw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3dumpbjpw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3lsaprnac.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3bggwbcfx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3asyrlcga.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3dbazqbez.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ecyusgfm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3boswcaas.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cfxfnhbk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wjakbktf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3onzcenrz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3stxfzjpx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xmybxvhc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3qfrwokoa.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3mgzirdri.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3dhmyvmbw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3fgwguzkc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3rnxrbqot.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wmyvqpqa.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3twuifsfn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xmwbtytp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3tohuflwu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3gkuzojio.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3qafjkdhg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3jxdqdidp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3poerwnhk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3isapitnc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3mwbinetp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3kkusadgy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3uprmwueb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3cktmxlut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mubcvlal.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pkisnukv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcpqasuq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bulmyaxl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pxtkrlzj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3lzecjqxn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3wfwvioof.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3gzgiijaj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ohokkwhb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3iaqccqwz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3fqtwpnai.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qmzhtmay.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3qsujbubv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3eawnnewf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hyhwsjik.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3okpvwgak.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3lctglfga.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3nfbsjvni.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3awdkktml.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3sjhptrdb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3pvgxtyhw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ovgsmseu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3achmstic.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3bgpcqdfj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hlsjvize.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3lxeecxjt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zeoeedhe.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nviozscb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3xwyrunns.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vcyqoihd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nfzdvdhq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3pruikvfy.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ftuwtqxl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tzfbtbpr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xznobbom.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3wkwjabpt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3eyktnvnb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tjjnayoe.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3yhmnmbsy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3eakaxzaa.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3fzepnixp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3xheocsnb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3jrsfgizg.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oyalbqph.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3bdgzfpyz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3lmmwsmue.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ifwlrftf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3vreybmfp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mlwpljdo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3mbjujtug.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xquyhpcc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gficxswv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3lyktcuci.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3xgixylew.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3loaiiqbq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3slysrimp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3guovbwle.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3lfdtszgq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3kcinfzoa.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3omjhffty.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3oqwqyuff.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3vbnzdqrn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3efmnmzxp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xiycamwt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hosywrju.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ujnvttvj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3tskjaydg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ryasmysj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3uydusmnc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3zwzeokbb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3jrccqpby.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3zkzcsbgl.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3wzgawtfj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ohwqnahn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3mfmkhhlb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qlpdatxp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3bqqwoftw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kauwfkrx.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3rwkpyyou.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3grfqhush.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qxnvwydm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3lmpjdxjl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3novxccpu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bdtpagps.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3hppnhyoz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3idqavvdu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ajpmatlr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3azoyuxxr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3kzagntln.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3jiudbmgy.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfngipmi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ptrfnhvt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3npekkrrr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3cokfvagz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyunwlxz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3izebqgkk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fonxhcjg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3cpjoftdc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3pvddvdwk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ylbhovzc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lbcldsdg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ivgxyusr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3tahfgwma.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3hjtzqvbw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lrinpodn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mgcywmbn.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3smdrzoqb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gklnkhsv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lzvrrsxh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3juyjpgmc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wobxsgll.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3okgvvfxu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3udtqqlrh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3llavbjhy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3yyhtobvu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3tlryvyzv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qcwtoilq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zsltxehx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3wxrldysk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qcstnfqy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ymkltecm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xnesicip.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3jfnzgyaa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3euqieces.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnltabhq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rbixkwig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xajebvcb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3pphjaxiy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3jeobxqzv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3bndhtoip.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3mfzggkum.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3vnrydaoo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ugzsvivk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3xyquazsw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rmlozkym.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3frpyhszn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3movtvoqk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ccuelpzm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3xhoioonj.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3vcrzirui.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3xhvtfxia.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3nigqyiym.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3knlsksty.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3jgjuccmq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jfvylgir.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ejcukogr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3hwxdehha.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mmahkefo.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bmmhsthu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3libvkxlo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3wfzfvcpw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3hiooqexg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3hagbjntx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3uzpjguma.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3qnzirngb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3sksyoqcr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3izxsalfm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3sopsbfng.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ctaryggp.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3zhtcmbey.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3fhwzbbty.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3diimsubc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mkgbrxwe.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3qtkdanho.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ahfykngo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3lggkvslo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vctmeoad.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3nzioshkz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3nxxsiigu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3kayaazfx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3kikwecrj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ddvmuqer.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3bkycslso.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3miwxvifs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ztbqzxsn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3bwcxgusw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3maulhhnm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3buyosgmr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3mcgheynh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3fiadpaog.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3pbvwwfqp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3mwukjryr.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3hqhlaixe.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3hmgioaos.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3vpacbnzr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yavjpkkl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rfetgvor.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ujnweasr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3tkfooicz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nycfimlr.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3nynbveya.html


<!-- 参考信息 -->