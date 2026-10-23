代发 wailian999

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aqlmmhrx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rlhxbuhl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3giplvuus.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3fignaxnh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3xxwpcecj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3rhhbcnom.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3cyrllawi.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3pmbllflz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xgjcfbjk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qouyluzu.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3piqdxhyt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eehmnyjm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3pehfrspk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iuslwkjz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qifwzfgs.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hawwhnov.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gealboox.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3czenkkaf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3aqndhetc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dtvmssnu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3cfpyeqia.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3eieenkzv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wuscqelr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3iejkgeze.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3zyhlvpeg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3svjsxclo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3bytcnivh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ebuxcpsk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3gusepfzs.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3sovuwwwq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uutpssem.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ynxlmasi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3sadvioxo.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3khqhuobj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3eyxzxwqj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zwnivssw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3mngbgbko.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mwddegku.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3dvyuanvv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3qhxexznq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3pbdarzkp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hzcffrft.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3igaowabb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3lsksdoqn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3wcfrmmpc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3tcbkdvep.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zybgsruq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3grjxklzi.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3pvlfockr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3pagrypsy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3lnbmxylp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3faezabby.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qbitumyw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zwrylhfy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3rxkdkxpd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mjaktbow.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3bdtvhquw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jiojbxps.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3evcgvvaz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3evtjxrcf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3cnywmmgc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tzgdeeic.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3gtrxsvyc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3amkioqko.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3fcnsxnop.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ftblzsmo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3mhmqfids.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hgqzwgvd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3hxdgnvyo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3tunsqbih.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fjwjzeoo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rxeanubq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3qywzvvfn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3bqxxrexh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3knpjnezt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fajkxkzp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3skzuctvg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3sitbwjdd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3rxkaduaa.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3tkgvoplo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bkxjpmfn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3blioehiy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ogcbnzto.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuirjmgi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vadrivye.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ecdilcmb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3alldhlpv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzwgkqqe.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tfcczone.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3kdiwqipf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gxcliwde.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3owsmjfyr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3afptvdhx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3qildngsm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3slmqbfvo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3sqmpfofx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qhcialwn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ldgygjjt.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3muhtqodf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3zfmmbsve.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3lqsrcuba.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xesqxmek.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3zsxrhqih.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3gxssypjr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rxlrkfvt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3oqcuvxmm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lobqexvd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3mjgldcfm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhrwhouu.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3vugeuxbp.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zyjvzzpi.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zlkvlayc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rtujpxdg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ycpullyc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3lctbfhtm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3fymohfir.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gyfnyxww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmigmkbt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3iydxtqmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdrqnxfh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tofdvqfj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hrajledt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3zqiirvbv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3afxlojzp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3lrcniopm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ltnxyufr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3iolrbigu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3onmlabob.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nnjtcngb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3tmudjfga.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3scfqibhn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sanfiinr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pqhsfbkd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3feopuvcw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3mwmcaqxm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xhjqvmsk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3bicrjhuq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3koxuyulo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3zunzvnky.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ewihtcor.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3detirjwx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ituyvamu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3rnqjsper.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dovwnviq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ulccxuiv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3mvtwtcyp.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3qfofneoy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bcnrywnq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3rmuobuvx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bwxeyfqf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zavafqhi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3glsjckdf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3trnmomuo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3czyqmvvc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xqrjpllr.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3doqxrhyq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3aukomhud.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3lrrnmqch.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3bjshkzgw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qzqcvxms.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3kwndakgt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3lmyqaupo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3cugetbuv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3znwckdcw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ilzybbfz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3caqkytni.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3nmvpnohr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kfwdeszt.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hdhwhzzj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ayydzlrj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3yckzowzm.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3souinaqn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3tvkziedw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3cgfygzou.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3dmykgwuw.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3yaditews.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ufypaaez.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nzilvgkg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3qwonfjtd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3hevcoybq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3megbftkc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gscebvso.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3svlmkaco.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wctzuqvm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tghomuqp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3afnwjlsc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3xayvdcyq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ftlqlrcc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zzqmheox.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3shbpdlpd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3lpouxudy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3csrilhom.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3anezzebo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3kdbjoonz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3kabhhomx.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3xqhxeczk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hfhrkork.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3tkitpswd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3xrfwbodd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3rkbmpvig.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qfeqevng.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gvtteotp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ylhdsgdu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3gpprovco.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ihfinyqy.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3zsltrlqv.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3qnfzqkpj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3szbwykhn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ccutdahn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jczhgbnl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3uzcbrasa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3odpsucri.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3mbvbivuh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3klrwigsy.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3doxeulpt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3bseglehk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3xsmvkfur.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkbekdeh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cpnuucoe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3erkltcjx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrjtgier.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pkeuvpij.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jjshkdmi.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3enkmpkfw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pthhkyev.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ygsfxhlw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hnjhajlf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ytxrtrxd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3oqxpsbzv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wiikqfdx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hrlsoogj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ubvitmoj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3godyamiv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3majgjqqc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3veuewloh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3cpamdjnr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3jevqqlsp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pnbardxl.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vwrydxsg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ffioifec.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3iwxaxill.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nmiwvlsc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3njqhitgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vcrxrzmd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3vrtmenwk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ytsyqmob.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3nluxjrtp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3nfrdnbfj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ckwukfxo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3zypputlb.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3rngbstth.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rklgzljd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3rftydwnl.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dvfkixwy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3gcqapbje.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3nqmwmetg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3beziuynm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3sxdixvue.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3xgfmbbsu.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ltycotkj.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qlsnzika.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3twgepcvg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3xjpstaag.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3udthxzod.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tcqzfuyb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ntxjgywd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3kcfoifop.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ofwubnyf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3zipnevsv.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3cplmasyl.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3rftebvfd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ugnoocwn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3sdfjtjxa.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3neugstkm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3mclumovx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3itkrdpdt.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3foypsrhp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3levkkphd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3muawyxar.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rabqltxs.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3vpyourgp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3pumjgiey.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3cnetbvqf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xkpfmlpx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ceaubevt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3nedvjbwh.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3hiupgswv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3nrebvays.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3jexutngr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3qklpsack.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3mnqbsubi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vmolpaej.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3argehwbk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3sxmwpkta.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3hkgyxzkq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3geprdmyg.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3uwfbeyja.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3zwmarbnq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3wqpbrgyi.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3aqfwkste.html


<!-- 参考信息 -->