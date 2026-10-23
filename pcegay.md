代发 wailian999

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3idxjyqbk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3trtzvkuf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3zrymqqmo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kzvutzju.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jolneygp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3afrpwwyi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3hfpjqdmc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ghamuiug.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3euojfchx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3aohjwvav.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3kimdtctk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3vhbsrviv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3hzervjhc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ofetenhb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3njbuwypl.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hpfxizgz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ykvhzozw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sajnarvp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ipohgjba.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3cdvxzaue.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dtdkmdei.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3wvdcrvkb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3uaqaefoy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3igezosrl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3mxajkqqq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3rufymlfu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xiayiyaj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3iydrirmr.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ezmnmfzh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iboilyau.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3wogyiaum.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gxkdfulh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3nhdpotyn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3qkellmso.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qzznxpqq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3akpfpyke.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lmdwticf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3yiqfoauo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3simywcaj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3cwkiodxg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3zsoyamgv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3hxvqxfjo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mykxmnsj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3zwopxzid.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3crlzkcos.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kvvxgaxy.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3hfspdjwh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3sjhpvouw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fvgrlnhe.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qyjctiut.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qmmbeitw.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3gngfmfgx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3cjifhzta.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3tisjrpdw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3tinmshfw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3abmrntfl.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3nultfvhb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3aybedrfd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3xjppuhsx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3okpsucvb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3wlybippm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3vkyagmih.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ffnkupvi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3erwwdkhf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3qsjpbgnv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gpcabfbv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3llmjzddh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlnbjphb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3sezdkvjh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lwtmdebz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3zdxrmkmn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sazavoss.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3bkxsiosr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3anhbuora.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dixulgwv.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zmxtrlme.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ypmivpkr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3gceczhqd.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3pgrffgzd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3pkukifnn.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3icdtkzqq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3pazfcnmv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ygztvlyb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wcyoatib.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ecjkhxmt.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kkhlkzte.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3dabbqjyp.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdkatfuf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3neutkuqr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ltdexvew.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3qnhormaq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3fsfhblgp.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tejplqwb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbnrnmrp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3icmspneb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3kitfmtyg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ofpkeffe.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tmzcchgq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fwrlubrb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3abyazfhj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3oqnrukwf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nhxfcshb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3osutriis.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3aqbsvndd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3itlyteto.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3iaqpxmdk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3esvurncy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3idtnokrz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3pbfubyog.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3yhrewwef.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3nfkjceyj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3qkgqsjyj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3dvakstmo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3tgjepqje.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ceahjlue.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3dahwnnwr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3hzaekbpi.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3blpvkopn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ygawuwgk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pyvxryyh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zevdmpgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epgynxpx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3aqlljzwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixptykbx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bokcuzjk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bamemdek.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vjezzcci.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3bswldgbf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3rtcvsqla.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3uzdaibwp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3utphsvkt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3xcvgfrji.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3yyvbplub.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3hanbptri.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gfxxogvv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3enygsuqu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gveglcge.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ekcbzhmj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wgnqfatr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cievuyay.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3rnyxrhym.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qvhblzxy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3onpovzpf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xpmycksm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vdvjbvdr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3kgmaqouz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3yrwvpvzm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fucycntb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3smccncwv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3kvvkftmd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3dwvenjqn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qlkwzutd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3drbvvqdu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3oevbbopk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gpipsjzc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gujtyjic.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ilmdstox.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qxgmmwum.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ygbverrl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3bhudnjqy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3qyhadsod.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3kyblmjin.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jcyoppmq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3rbqpkptg.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sxanbuiz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ksceidji.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3zrdefrbi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3eehugulk.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3mozlduie.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yaqvvaww.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pvlqbrtz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hgvybykp.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3gowluzre.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3trvqittz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3gsxarnkn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3bczczuxp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yxbqfbpi.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3jjkfvcqg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hvapicny.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3vfbfsmkz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3wdutfwnv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3pgmtvlgk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3cduptfzh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qdwbhrim.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hsmbnzth.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tthronap.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3xryisljl.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3onjtfmaj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3usqprjqi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3cgzrhkdr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ndtlujyr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3kwlieftr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vmdoktoc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yjfztbyg.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mjjnhdka.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ewfwsmpg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qtjfuaul.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ztbrnjqw.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3xxzgtwil.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3hqbxqwmw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uszpfnze.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3lygozwpv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3nvlphkkr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3tpwlprsy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sobumuxz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3xmebrjsr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3fwnkicpy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3jshsfjko.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rgpsvehn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3kwrtitdx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qbtgxvcm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3lvgthjar.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jbzkerfp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3folfjbpx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3vrueufls.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3brqubcwl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3srvhuxpf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cifydkau.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3upfkoxoo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3xaqrcsvi.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3djlpqbom.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ofbdriaf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zgnsdcha.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3pyxhhiwl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3gpaqtujb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dgvjpret.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3senuvbyj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3eiozyfqx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tundzdve.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ampvlyty.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wellznwb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zmcbtjsp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3kkxdpzca.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wdzdjhyf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3amxacjqk.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3causjski.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wcnvygdc.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gvnoomdp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ncvijida.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3xuucsijn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ugjcddyr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ducfuzgq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wakvzqnb.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3wzsnevra.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ehufdjcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtenhogl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hcshxhyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etcpavuk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3tnerjanm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3rucjsqjc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3wzadeclu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eklqndcq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qluzynaw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3dlxznfdr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3hgggisiu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3yvuqmktm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3yhbqmzwb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bmhbjwxp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3jgfhsary.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3haoxuzzm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ocrkxnla.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3yctujpqw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3yffdpeec.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3hhtmrtvo.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qtowffba.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3lfmajgte.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3paxnjhcf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3zswygsne.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bozbvdfn.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uqjajgbq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3zoxyyvzb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mnxgkeae.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3xwneetkr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3wqmupwsv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ecjckbgj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ugbdtumc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3yprmjyqy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3lgrlizyx.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ehiowgcq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ndmgwthm.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3eolveoni.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ttegyhfv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3zkqsuljl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zceobudd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ezadldvh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3gsfhpgkt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ulxhcfej.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3gafofegg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3jftfofon.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qrasfqjc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3hssbycow.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ekwjjbty.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ghcbdvof.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3zxjgowyw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3drwisnsx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3oidnvjlb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3vvwanbva.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3nedkgduo.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ijjziwjw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3xispmxbr.html


<!-- 参考信息 -->