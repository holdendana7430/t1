代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3rydtmepm.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qdmcvbak.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3zlcqyrnz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kgqikxjd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ovbpfolr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3htmdrfgz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ahhyislq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3eymwtvdi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vbjxviai.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3psevmytm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3eeigjzbx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3izdhcixg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3wsxhykwg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fmqswpdo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3genytvqh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3yxmwdnft.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sapgeajh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fsjreyfx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ggcdevvq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qimijolh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3svimwdcz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3udyfwcba.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hxydetxw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3cbpwvaao.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3prdvodmy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3wwsvjhdc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3irekmawj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3znjiaamr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3bjjiymus.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3zkofeuor.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3mrceceaf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3stjiumsr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3vcckvcom.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3abaggxfh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3hbebqgou.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3wufvrdkm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3wlhddatv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3yrulwgzt.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eyvbfohf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3axyqbtuh.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qjypromd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3gekeglfm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3onnqvara.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3sgdwleqg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hipzlblk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3emxlnpvm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3hwomjles.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mmsokmqd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3mlxwohtz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3lxjvgnma.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fhjforoc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3znlptkvt.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3sdwxujgq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3tevotlxt.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3mvzhfyer.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3wwazjwwm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bpjijvgr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cmzlysxw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3tzcchfyu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3soxxrtxl.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hwfoqxqv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dpvnvaur.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3cmvmjunr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xtmtihcv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3jwcrcbyb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3aljgditf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3qskooacy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3imtbmsdw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pzckljep.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3jsanbrhk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3lybdrlxa.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dsjcgqhh.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3lyebjeay.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3sbksphig.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ssyrkifn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3suuyapbt.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3nnezmntm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3dypdxyrx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3yactgqie.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyquzsid.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cdtnbxtl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3aolsoues.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xwlxuktj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qgtcekeg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3rbwzblgp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3gdxnhfor.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tduzswyp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3rdejdlcw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sjduslaj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3klzhsvjh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3nzxlztsx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3nopinoti.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3esyafrpr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3cjshjhsw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3pvimnehf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3kliyhbmf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qnyyqbmu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3oacujfhd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ybbmgddc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3hbkcetoz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3tsmjxuep.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3fgkjjxli.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vgmkhygn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rwhhazmg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3lgcznewp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3fruekszx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3knowmlvm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3bshhhsok.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pwjggkol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldrkbjev.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3uztdtpja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ybvsbahl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3puwpeebl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hkifajdk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qiabrrpv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3brfrnvmh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3xtrfvjui.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fnyjkjex.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3wfbsqgjm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jmsjujqj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3aerzeaiv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3aofquuqf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3weajzhoq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3juomzdpt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xijehtov.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3glqhnfqt.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3djwprohp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3uezczeuo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3vqbseudv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3xmgfbwvt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yccfbmwn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3piryjtow.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3mnyfeopu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3phmvrkdr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3jvhhmxya.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3trhiajcm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3orajnzjx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ivyvwfrw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3podpdcpt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bjslzrpv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3bbrffark.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3tehuawhb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yhabmdzz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3focqbyzd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3gohbhnoy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nttebbge.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pcoqbvwx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3keszzszl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cmrpnbgd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3mkgjckgp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3mnmkvhpe.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3wxmcypcn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3lvtanwha.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3gzmkpxxs.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3brhjcxvk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lgqkdcam.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3esowqijf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3jgjeeeuc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3pqocnygj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wxggefkx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3urftixsd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3jzrngtdr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3scizocts.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qktxjgic.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zcoopzsm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3nnviyxnj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nzvnliwq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3iectauzt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3kzulatni.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3lilavysj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3kutzqkas.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3lyhonoqz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ywichdll.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gptizuol.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3isaacuxz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3dyiyujzr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nwhbqmag.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3mrdmvrpt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3xcrhlwtl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3wafogyog.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3wqlroxao.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3xllvrper.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zmpwhlsr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3xlgzbttk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dwwugpwq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3tvhcuhid.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3leasmytm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3upjfkeig.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3brhhmxyb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nfhuqkee.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3bkinzosb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3majhbdns.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lpavwyhz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zbsmqlvr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3srhozvik.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dhnqqolh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3atcnlfwu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ypakqrfv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3oevhnjgp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ucuhznoy.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vphuvuzt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3iowdpnvt.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3jsupeajp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3tzfvoqor.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ryqyvyfk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3syluljqj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3zgmyvask.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3genzcrgl.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3yaxfucmf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wgcccnih.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3aaeviebd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3zffyturg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3cuvriwcv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kgcucfxg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oqaaobop.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nznjffbh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3wjmfohlf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zxznbiqu.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vfffrprj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3sboclrou.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lsduaahd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vsywxvls.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bcgoyydr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3unnkagio.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nlplsipk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ozmzgezq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dqffjsap.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3mfihxmot.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rtffxiww.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3anjvlkrw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nfcpyofh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3btyfyala.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xxnmtcjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clyygwpi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ijjfhczb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecyakkne.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ovpzzlni.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ubgsccxy.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3tenywchf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xmgsuoxh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ofjqfxjl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3lxkrqpqf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3goriuzyh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3iaiuvhtk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3uchjrcrp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3irgcxlrc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3dufxnjjo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3yasxvbgd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3oniheitt.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3yqorarmw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qijwllmi.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3dkqvzmdj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3epnrjokp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3reclyvua.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ndroscjg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3tjxxeooh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qojytttp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3eifleehj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ebhdpfho.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3vzoyomgn.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3kspoelon.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3chdzjdsy.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3pwazafug.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3klokzadx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3qxuiplxl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3kviourre.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3mjexkaig.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3inxvhcji.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3wfzrwxrs.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3shjttbsb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3nanivqad.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3psdfollm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3obrxrtld.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3tkqcogia.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3lmoacjcx.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ickpmako.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3saqnuzzk.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3fzqjjehj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3pwuertvc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3jpjlljin.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3tzxggtbl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3kawhwkhn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3amjnaoic.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cgqttbep.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3jeapvkxc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3wcqhkves.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3bxqcpppk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3jcyvuocr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3vojxynwp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3rbzfbedw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ueebprgy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3akhixqrv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3pewewved.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ubusexoz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3zjmzypbw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3juowjekw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3nvszyhep.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3bsmxppms.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qatxvafw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3zjztfdon.html


<!-- 参考信息 -->