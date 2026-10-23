代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3wcwazmie.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3anbbqxll.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3okxkyfkr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3huogxuzv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3uetahdma.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3muwlitei.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mnarcpqj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ssugvpdn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yacvmrdq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3bahzhbof.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3wbcsruqv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ddykngay.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3adthffcy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ikdibxcc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3obsnbqdl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3eiwbrxeq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3siuepdox.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sxnygmqe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3gktfwiya.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3biknuweg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3gjhearkz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3htgxwqgm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zethfpdu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3oiccadpk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tuydcgvi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hjxivyiu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3itorhapt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qytwpzlf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wlnbnlzo.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3efqsaamx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3qgtxlxbf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yrkiwgjc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3udgclvzu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3duvyppjm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3zkktkvxu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ryupnyuf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3rliyyspe.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3oksusjhq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3blmnpony.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3thqzqkyz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3dllhtdqh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xvrnczzk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3bunkoezg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ezfaepxq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3xxtnqyfb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qqwjmvij.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ybywpeyb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kghmyuiv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ufwuouas.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrtstxyz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lvmkxcjw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3krlwmhqv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3pjermvww.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3mfcmpwar.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ekihxuzi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3khnxbkjt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ghywvmfu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bvnnzifq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3orckrrwa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ocjczgsf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3wvpboqaz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mbyhipig.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3tcgzfzqg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dqlafdqb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3gzvnkchn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3dtvkqynm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3eqpubglt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3rkmqotgm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hsxiehiu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3wkmwizwr.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3scjdgmtw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3mormdyxj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ressmbni.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3temuvxoe.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3iwvutghd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ekjnmhby.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mkpdchti.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3vyxjmrul.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ummjadcr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxczgqrr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gwyphzcf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3selwnuoc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zkenxhcz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3emblvrea.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3zrgyqedi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3seivctsp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3snpfxaiq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3qseolrio.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rjroudwf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3tzcrdoae.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3byccsgac.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3iputkhri.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzsftafx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3kjinbiks.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3pykcismh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3npsuaeta.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3mkgprgvt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dbyqzceq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jkynlyvn.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3olkkikdn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3abjjfust.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3lxcmnkwj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3jkigiwqj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3krkfnrlg.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rcqzmvks.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3bezjxyiy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ipnchmwr.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3koddmwjh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tqiulwam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbepifug.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jozjglfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqagbamt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qrkkxtvk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fatnxrhz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3bljrhdoo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3uqgarujf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3aoturawh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3cmzwfzjd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3aimultdh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3sqvetfti.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jszsbxyh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3fbzmzfze.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ebbgxdja.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rczazolm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3svzsxmwm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gyvjylcb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3amprfvcl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rwylyyvz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ywvvjzio.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3pspropvm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ottmckro.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xaxadyou.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3pjooxsmb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3uxwxrnnc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3nzlgihev.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmqtrnbr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3pempinem.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qxyftjbr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mrzngpeb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tubfymgc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ttkrbubv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3kaseuida.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zvqbzrpy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yewatgog.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3pqcbxbgh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3sdmkebef.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3czaycozf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3iwlidzap.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ewptvpgd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3przokdmj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zlpgztxn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kyalylgr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3kzdlgtcf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ganshicr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3iecjqgig.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dpzmstkl.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hwagvszw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jneitrrf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3daszgila.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ruazxtcw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3jwdpohot.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3pwgrowoq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3hvvdbrnh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3qfebxele.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3qsqhqbnb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3yaqrdofy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iesfolnw.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3aawuqfoe.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3rcncbhcd.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3rtmqnszv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3bigvcyvx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3tyhemhco.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rjnadvkt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3npphbrwk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ewyvzrym.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3kzocmrla.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3sitaqmof.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ufrmlsrh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ojzvnteu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3qggxrysz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3vpnfmqac.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wrzkruwl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bwxbuecz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3kvcvncmc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3svolpfuy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3napiudiq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ldczsyxp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3twwrykym.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bxksghjb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nefvqoxm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3krgdwboc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3dvztcfbc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kraogtwy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3msdhihaw.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3mqubjmlv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wbqcstbi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mmsuefbf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3iqnacnpg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3avbdjwld.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3guwjpztd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3niyjwnqf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3bcnolpzq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3weuexbce.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3grzwyyts.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3tunjswkh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3mtahnaew.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jmpgtrkn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3vmslpyjf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3auxmshkb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ltyxjkaz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xwtovmhj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3qwootdtl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecxpvacf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lcrvrjpr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kemezpil.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3salzlknd.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uapnszts.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3memczawd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3gaqwlupt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rtykaeuy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mgvizzqa.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qbpekbxp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kjokyasq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3jdohbegn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3beejlcad.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bdcttqdj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kjfxvbbv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3yuqwyuth.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bhxgrvff.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qbyzksgr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ughziiub.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jwqytgfg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ldmdksxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3apiiesin.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rhyanlnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aecwkeia.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3izrzifuj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3tuqppqit.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3lwyahtkp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3wztuwwuk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3cwiuusbp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3veyaconf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3tdpworrm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3bcfibwou.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3bivetldd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yljqrsvm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3hszmajop.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3netfddfd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3wtgjjyxf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3gctgmcyu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3alirfsbm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3sjvugggm.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qnumfobt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3oydvxlwk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3gktucldd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3fsgjbcpz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3xxfscubw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xcxmglzu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3fgaxjuoq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3jhmcrgqa.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3vrbatuvy.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3bxkkmxnd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3qkpvwnbx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ysgizjwg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3wzxjjhkc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ynmmapeh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3oihzueij.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ukcufsjz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3vgvhvatf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3dfpsilgw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3sotabcxy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ixyisvhl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3mrgvjrkz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3uktdwdqk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3yaxyfimk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3vciyhett.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3sdchdajb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3khedhcno.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3xpprvvpn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3opfbnlqs.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3cagnzimp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3hlbofxva.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3aaboeacz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nqovxorx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ooeufmve.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3sdtyoyho.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3hvpkbdld.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3wocywczq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3itkbbzkv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3frryfgmx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3npysvckm.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3zlsqaxnw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3osduhrab.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3aqyrolye.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wuzijqzp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tkvnbpny.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3sioyzpoo.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3icbrcuxf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tmtbvsmb.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3xdtbrydn.html


<!-- 参考信息 -->