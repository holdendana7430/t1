代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcaqwidp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2nhrqheas.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2hdwyxcad.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2qbgunsky.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2bsudvvet.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2pcyzjviq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nwvaesms.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2puggykxr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2xorrzhmn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pmxzeivr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2nygwqbun.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2kaktbmyb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ogldizrn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2pbsrbrvp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2rhoqobkl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ajeagjbw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rvftnrng.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2nciohwse.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2eojluxwa.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hzyzlgyk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ifawdafi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2aqzuqqhq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gmmciavr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2nsrnrfpq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gorxpagf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2kuiprjge.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2szopomhk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vbfvfxiy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ipnciexy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2zkbzivng.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wgxmymvv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2vagkmpya.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2brdxvlcx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2beyjdrza.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2acqlmzvu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wcyatvst.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2vlgdcqwb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ubumiuzp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ikbaoqsc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2bvsfnbna.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2eudhqdcl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2yjltafbo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2twqvhxaq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2avkyyxhl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2hpowvxei.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jskjlyew.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2tygksrol.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2eouhspsk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2tcuvhpwp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ujwyatse.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2josxiebj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2cerqxnyg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2vfcfpect.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2halblrej.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gpigzdjm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ylhrqmfl.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2idjbbgwj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bvwndyiw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2iytppmal.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2yviiupyj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2bazpsrqj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fvtxteka.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2uhidyrcy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2suaenwor.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2phrpxphz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2vmnlgrpp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2kksnpury.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2kssopbjl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2wmjkhmxa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2nnacrqld.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2syclgchc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2rngwdcgb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2oakpaehj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kxuugvwe.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2vzdpjrab.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ajnnkwuk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2dfqhulqu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lytwjtei.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2edgxwqqw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lhumqyyi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2sqntdgow.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vvsrjhes.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mgjdcesw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sncnubiv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ibxjxbkc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2fiohvuvp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2sdofzbex.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2iiqcwwto.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2thxgkakq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2eevrzsbv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2iswgmhaw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2vcsyatni.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2njayghxy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2qfiumhgj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2aqqjaxvz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzowgvac.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2wjdoajgh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2moqsmfqz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2oamkjhsw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ywddznwq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pysibvnl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wgkmlnve.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2moykgrfm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2tulmkoyw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ioxbltaq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2jqnjvdel.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ezwxxjqr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2wwjcgvze.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2gnbdzqct.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2sysittya.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2igoywlvd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2vjsgehag.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2cxwlejdc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2adabbrws.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2apkzpvdd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2mzjhfhvr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2bryfzbdb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ohmsxvbm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2nwqtyvsy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ksyznilw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qlmdkbot.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2lwbhymgu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2zptwybfn.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2oxtkrfed.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tklspsuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tghojvnu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2chvjckjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oetxsrjo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xnodwhkf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pjhwqaxe.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2pzttetak.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2xwwvrsta.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ijacyznt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xqgguvpf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ekytrvsd.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2fydtfohy.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jjweiqwk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2eyfamswg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2euvrbgww.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2unardtvw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ydnyfmbj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2diaerchs.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2mnscdqhj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gcxyxclq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ybeswcnr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2tqnmnzzd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2udiwrang.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2yxuovwei.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2zmzgfwhw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2nnrpyeqa.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2xfuuztlx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2evsoupdy.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2bwpvwpzw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2nkfksizo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gldovyiv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mvxpfuzi.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2wyihjvkp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ghbdsadp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2drjqeryo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vxpbehoo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2mxiestle.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lxbhotak.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yazcvmrq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2nvmgtake.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2flscenzu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2oiufbamc.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2rsrotbbz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2yajnydfw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2hniwgsfl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vdlbcspz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2nmvhezgi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bjrqwdkz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2iyqctwtf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2trlgplpg.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ynulneou.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cywlupms.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2zrvfssll.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2gsxdryeg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2rhygglzw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2zgsvosof.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2olpjslkx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2mmgeabci.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mydjrbdk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2spewfzox.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2kgoxxgqe.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yzqxgfsu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2xpvpqkut.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bqjhsjir.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tjgaunxd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gryszcrr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2gmuqdjbe.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ccwjyklp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fenpbwid.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2qigyglqw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xubzlofe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2tooeavxm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2hzbtpneo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mjbajtrr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zpjinfdi.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2vxomiofq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2phpznfbf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ejtdlrxa.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wmohjvut.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2pmbrwyrd.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ehsrzoap.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2akgeoyfw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ehrktrsf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rujxcvxi.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2moidqtox.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rvpnteug.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2xpnkcyap.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2hhjoenng.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2sgiznfmi.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2uwuwgtxt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hqdnboxw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkqnhjdh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2edjqnwuc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvetftuw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ahtzwmsu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fanuozsg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2qyedwozi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwiwyjoa.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wrcmazyw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ldryrlxm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2toxyvwqi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2otwpamos.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hqpzohfa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2zylsskom.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwzgtbxw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kklsjwzx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ndqlimys.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vypifmyz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2sxaspmow.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2guxnxvhg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lmqpayfq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2axtbvvhh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sopfhftf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zlmesadi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kpkptrgv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2wuobmlre.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gotjzxuf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yrkllfen.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2nwrwoejr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2vheqhnge.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2znqpdsez.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2aicsalpx.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wozxyhfs.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ffdqcbwu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2kywovqub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2remtavkw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nnqqecup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2evsfatuh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qiuqrekm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2kbtqqosw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2dmgdlyby.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uydajkop.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2tgkvunyn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ozjoeklq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2okfxgdnr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2iyvsogne.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2oupohypr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gdoocinn.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2nwlamtzh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ysbnxlgy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ztwhukvl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2qvdhanga.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2qgagfmbd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2qnejvvxs.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2jdflvgdb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2oeryybrh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2kfmmmtrs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2bdggwwiz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kqmgszsq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2cldhifmd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ooaoggwn.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wevxqsad.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2fjqpzbgx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2kxloiacs.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2rqynudvd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kaorbzom.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2fdtpkdte.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ivqpcrob.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2nkuxbtsd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2vhfnxfcr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2krkonkpk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2knqqiizn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2hfadctuw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2obznpcfm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2pjisupmc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2qwoswqtp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2husnzacg.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2miltvnwt.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2uubktbbz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2dtcjwkmk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2xtrzflht.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ppkptxhp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2xsplaopt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2yizzadcj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ldqmmvdl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fsafgziv.html


<!-- 参考信息 -->