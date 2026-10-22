代发 wailian999

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dbswtjps.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ajcscofu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2lrpnfvrh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2alboljee.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2lxcsybxg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2whrpiigd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pxksomol.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2igpednpw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2uefhngzh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2hltstveu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gufhytpl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vafjbzms.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ymppknra.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2erpgyfob.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2opfplxbt.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vzuojttw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vxbyogsn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2jjmqpyfw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2pbmumuby.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2xtcszbjf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2laetmlqs.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2evnsekei.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2arqczgyf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2dkddgkul.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2zoebcxfr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ykthpzwo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2jdwwcivg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pkrgdypb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wmecblbc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2odwioept.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vdxkqwio.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2woybajvm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ksjswbml.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2nnscuxsc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2homxaihg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2fgdpvvvr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2eogpvcyu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2pvtitqhb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cwliotkq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ljljpnfj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2zbvwoyrc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2anchjgmu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2dasstqaz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ojjlxegk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2vdbepvwp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2lualxeon.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2karziajb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2gtngisoz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fentdmly.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2iuuybudw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2qcxwwlbv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2cvtjbqnk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qlnsboig.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2hrwdycmz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2afgwbeba.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ccslevyd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2edwerxjz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yypwjans.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xgweodwl.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2mdvpamvb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2hqjdxhqf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zfrnqxxr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2wzibmojj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lvbtjwlz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ttxfjwva.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lkxpjwlb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2yhfdugso.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gdnsoohz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2cjiajhmd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2dggbdwvq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2asngygtp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wnxqyujw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2qovqzgoz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2eidohhvm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2eyzqyhtz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yfryaesq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2hbufjptk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2pecixfqj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2yprykxuk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2geuayfyz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2zthhxetd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hxyxytvh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2vdwszhst.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrirgeez.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nhcterib.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2khwjhium.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2zpogbdaw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2limnkqcj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hyhqtizi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxyvmrkk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tpjqhpxz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2qzsfzwti.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2eqnwyeez.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2meuxttzm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2zxfkyism.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2bozsvgiz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qnbnbyje.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xesxbatj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2lmasjbmc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2fskmttcp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2pexwxfpq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2jjuqjltn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2sptakffu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2eucsnnpw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lfnboips.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kqighaxr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2zswsvozh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2zufcvwiz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbhjrtbp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2eqicpeyi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2xewbnkzf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hmeseyse.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2aizxlwpp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2nijdrcyg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ymqlxfdc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vkgvglwu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vinueruj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amivevxu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2uevtwlhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdahsvca.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kndiahcy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tzyurmex.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2iqlpoymg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2bbcynejj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xdsefkfo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ixuwaumk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2gnevvnbt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2tqutwpjj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2zlwxvnoi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2rkgsltmm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mjpsmlij.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2goplttbv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jrjjcsjr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2lmvczaka.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dwxfwxkk.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wnwrjsys.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2zezkuzqe.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2oerxtdov.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2tfomfbcz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2gqsxgpjr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2swoihcsh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2leaexpcv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2fxdgwxnn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lalmxbtj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rrdenubh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2dkkgqfpg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2aovvykmw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2uxudxyan.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2xamvrddb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2rxrzsxvd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lewcyfuc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uazbrnmc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2kvhdjysg.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2urnzvhij.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ghsrqsth.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2qtgxldfj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ivsstemi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ucisrzjp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2hliosqxy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ycleutim.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2tcmdzxpr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2lwbnctet.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2svxxjdvj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jzlhxyfq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rknzrmyf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hniyzrge.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2usparxwz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zhroaghw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2cyhdtrgc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2rzebccax.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2vnlfxyhz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xwolksll.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dgxgtspr.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2dnichrbw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nxkhpjgi.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2topalcrm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2acnfuvqv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2eatotpge.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ocyrmbcz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xrfkdyxr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mcynphef.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kczbkivg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2osrjeihg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2dulhdvjg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2piiyimpc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2cqenqcdt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2qjmavlol.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2muwzxmij.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2yrdnfnea.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hhyyuior.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dcabviru.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2uigfxjnt.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rwsjcgvg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dcdwdexg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2zlrfrbjm.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2cqrmhrxx.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vvamqrvn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2hawjslrp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2jytzdjyy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2lsugchxo.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jpxsovcx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2tvrxwjat.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2acvpveyk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2clhoddnv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rntxkbmp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2uqqliuab.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2bmfeqnxk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwtwdkrx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wckcbjvh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2vetrzfng.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2lmwgtcsa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kaiyykax.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2qjfqziiu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqjpbjzl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2yiagihuq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2fxeljaow.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2wxydpzai.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2amohgmcz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yogoagah.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2fkfwtixp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiqgexbi.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2egejjgoz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nvzesyce.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2detsxkxx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2txxvfeek.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lbqypppf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dfncfqgz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2sybexzzo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2huqwttsg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pxfxjtib.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2sldxvwyw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2khztznzg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2izvximda.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kevgapib.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xlehsjfb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2rngelgfx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lnbrqzzo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xmnxkaar.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dbwvzsgj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2jsadvyex.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2zcccnedl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdwhldfg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vqekocqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xdrordik.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2orffynoh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2gjmhdtfa.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2rmlnepcq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xgemznqe.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2fryboeix.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2jkjqzupn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2bswuxhsv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2zwlnnoth.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2iuoblhob.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jivebafe.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ipunatsl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ivzdtkmf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2obdflear.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2qibthfjd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ebqgbzwc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2yppsetff.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2igsvirdd.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ccbraltg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2vwjphlas.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2nntjaqqy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2yjalqdzj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gbpgdqma.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2qmxquyrl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2medfduxz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2kfmcrzsg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2teaskyco.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2nwpnzdqx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2bhmpyxqj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2xsobsjcq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2oeelufiy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2qjpjkihc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2qontlnts.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2qogbsaei.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2mfwqxiwx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2cfkflhfy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ucipbtte.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2mgrrkqnp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ytgwvljz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2pqpaekkx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2slxzbqmc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2rzimzfvw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2csbggpge.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2cmwlngye.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2djngpzjn.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2thhdblks.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2shflmpac.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2nshsjbtu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dhzeogpf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2zyzrthil.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2coaumehc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2jkbuesbd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2farwfqsd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2lmmpqltj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ufqrkbcl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ofsicndm.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2rfdqauac.html


<!-- 参考信息 -->