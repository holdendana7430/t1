代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2bigfkvsm.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2cfanwfum.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yhconnln.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tjpudeol.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2fnsrfuvt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ufddsrhn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yczogcoj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hsfflrsn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2spvxpobh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2bfedxavd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2bbcoplsv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2wsuznfzf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2skelmeod.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2fryttbrv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2hwuvllmb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2choqohht.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ufczzall.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ytowqozz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2mfkmhfjb.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hngivhry.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2hsluoaxb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2dovkhgsf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2actfgolh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2jzlbzqxc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2oqccukxl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2pvnqnnyx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ctaoesci.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tiigsrzd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2kfrjnlgl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2aatuqrmy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qjlbktyn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2xwinjtzt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qzqebflr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ljhramnn.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2jtgjiclo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2egatecof.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2orwtoqvs.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2vpoybdjl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rkylzlqg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2onhknfgd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dyrosyvl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2eefgrlwg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2mpheetgj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gsmohnkx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wqhkmtxk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2iitokvxn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2suhdukls.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qiyuurvp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2nldcehug.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtnrqgpb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fpopmjrz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ofqyeewe.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2tcdmkwub.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2linjdmqc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2iinvvryw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2syhdbetu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2knyzuays.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ikbkfgtu.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ukbjdquw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mspdjoek.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2dsfmhpgc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rycpvewt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2qsxgaole.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ctrcjbrt.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2gxhoayqk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ziflrcip.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2itrdgtir.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rlhqgthr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sdabrwyz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2fupcwrkl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2nskjsplz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2wobjvmom.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2gvhuqlbo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2mruwvsyl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2anfjskjr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2gcvderxp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ghfhkuzw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wriqcjgm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qzufkhvm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2mltmdydx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2djrgdqvt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2mqenzatp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zavcsthq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2jhcwbvea.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2rmoruoiz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ryvirvbx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2pjssfnsf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2baucxbua.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2djtvuxxe.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2kuqscuee.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2oeajzyhh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2skvxnohy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qfwgxrfc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2rttigbvu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2fzxwzwrl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2igvzctkn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2qbkmkpqi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cultgair.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2utalsflg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2onegtzdb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2qnyjewtd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2khtgyiaw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xxvnxhxj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2subpzsdk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bpuzbugd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hrqulyem.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2dzbwgfcf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ksmpjetq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wilcsoyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agqnhaqo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rghxscsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulklobfv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cogsdzqv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2teyvfprq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ewxerofw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2gggituky.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ydzdzwwn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2oahifdte.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ydhppvbt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ikpbalke.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wdtpzljt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2sxkjkhac.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dwllrbpa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xrznzuaf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2nmxpbebq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2foxlderg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2mrqmwump.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2eorbpjzy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2oseqlfcp.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2acmpsifx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2urlzfaei.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2sodssdll.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2digkezhc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2aoncwciz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2cbvjlagu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pkfitlhz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ucumyrxi.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2rgcpbarl.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ojqruzgb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gxfnyujh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2thiagstv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wjdqvthq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gtpkqtsc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nljoqklg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ljwoohcx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ynjanzky.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ticsdkml.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2atszwdxi.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xugupsnk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2wbaatqbm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2maotbpwx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2foiqrzbv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2leqypbcr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2mrwsgitv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2uszhfjvn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zdcelymx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2memvbihl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2utqrplji.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jjdjvilq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ouuavdpj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2zjiyqkbo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2zwiifvgn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pnvqzreh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2sbkxnhmn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2zbuavmak.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2mdrxygke.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zhuxyxat.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2npvxkkqh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2tylfyrnw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wkgjfgxa.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2fpnlzezl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rxpaibbq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jbeeouyg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lqunlwvr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jqqoewkl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2eyhxcxck.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nzhlikgs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2kcswutdg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2oaxbeyff.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2mzqgrbzt.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2aebmpcgm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ejywzdcz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2kmfoxrrq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ivcoxqzr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tkhgvoom.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2etopwxbw.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2xgfyoyow.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2sgquftzq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eeyuckej.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pzaoxowv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2woqgcdxe.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2mpeuntwe.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dghtegic.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ouhtccjv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2mscqupgg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lvygyerf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qvsvoqqu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2phivgwcj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2rgovwfkk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fssmdzwi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2axcjaxjp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqqxgqxc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2lkhhzelz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vxgzhnld.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2cgxichuz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2xccbtfrz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ksyikqje.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2uurbojlo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bshdosfm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cciulyia.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ngmpwkxq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2kllaqjua.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2lbtpgcff.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ctmdmcyb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gpidthmh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2axzyitoj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2kxbulfjr.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2faczyjjv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jlzhprxm.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dzrpvbgb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2oibpyzjy.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ordhzcbl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eldznhln.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2xopuxejj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2oncxnxqq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2koddlzpl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zxbwemjg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2vkjuczsp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2geazbtcr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2wuziexdr.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2maiatfek.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2kgkpayew.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2qdnenmfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eczoekgk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2cdssjpia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smbyyqsg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qvppngdb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ishnhicg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ciakvbfm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zbpiewhn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ufpxncco.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hhvhkqhl.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2segnxqxg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ndhfpkug.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2livqapjo.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2djtxzwfw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2toylyrlg.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2eqifqfvr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2tmnvwkso.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2sfnovivb.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2vhxumjgi.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2cwrwcnjm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ynxxsqyc.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2cmdxctii.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2erhcdess.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2cuhrbdbx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oynzsnke.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2adycmpkg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2dgcpkdok.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iuzpogdv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2swzpiteg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2twnalbzk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2dtrnharb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hjzejjlm.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2auizpwzw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ydioynad.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2loguyzer.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2yxiwcfir.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2txfrvrgy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2lihbpbta.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2peeyxlfh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2adrwvrdd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2vqpkllva.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2roqsjrqk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2dxbpomsi.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2eabefptr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ctiofeuj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2otopawoh.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vbzleqjy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2aljpmgmv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2iycvzkej.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qaaoqvoh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ikwypkth.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qaemabks.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2jximgslq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2jflqjcae.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2alrclibh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2nvrxfngv.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2unlxelyb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2qjkjeaje.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2twueuqbw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2rrwuxtmk.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2uxrcmenr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ujhrprtq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2mnchcosm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2jibgdtia.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2mnopdhkk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wjvcreyv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2lxtaxngt.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2tnsdsaeb.html


<!-- 参考信息 -->