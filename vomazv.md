代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3bvmgmojh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3cbiykqch.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3oyoivbqj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ggwxcvle.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3momjoazb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vaphzhmp.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ktdavrwd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gpbgwrld.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3wnyhpfgi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3wwgpchia.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tnuheeue.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ncrykrsx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bunpesgs.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ytzchkqp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3zwjxwmcn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3zbzlxodb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3gohzbkyj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3mdyrwuah.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3emujucxv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ehcpcdtb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3wcuggvwy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lwddnimb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3tjpswewe.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ucpillwl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3bdrkvkhe.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3hbnqdsiw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3kapobtjf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3fiaecrkb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ryipvpwq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3cdcyvxzh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3qpctspvn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rijsrewr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3auoiytwa.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3nsjhpmua.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3hvlarqsv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3vxkmcvkx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3btgqjuxk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3mdttqgvo.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3bmwjhmpz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3mwbmexgv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hbbxsohz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3yalwgwun.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bjtynwmr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3jheywxes.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3odtxxicc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3audtxncb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3uifisxef.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3djyysdrv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3mxagttms.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vdzialsk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3muvusmdq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wqmevgtx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3vhttasvu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3zxxxpkee.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gdfxusqy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rktbwhmj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3lkatffgb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cdxeczrk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3gmrnvkcz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3edllvhpz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3cgkugdzi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ydpqhosp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3yhmihbvh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tmeurwjm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3dvvvajqt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3gduibovn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fuaaugka.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rycgayet.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3gybdydrx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3qmbyfrtm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3scdsnrkl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qmetfzeo.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yujugwun.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3iigurncy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3izixvena.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3qtjfrrzw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3zxedigdg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3tnqsnaoy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3wfxtigbz.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3djubmmnk.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ecxikiam.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3xiyoxyws.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3vdpppmay.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqqeqjre.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3urrkyenh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3tbmzxqur.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qwfgfdjs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3awqfvtnv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pyvlpuvx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3zobwsayd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3euhzkjci.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3szlncjfb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nyaylayy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3dzsyqlvu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ezbngich.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3xamtpaeb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jfcxalws.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3pazkcgwc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ixconjhy.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3qzhwrmsc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hauakmgw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3devayuyp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wkqcfoag.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3jcbvsmyk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3mndlxtix.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3cutimfrm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3fowgnsor.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wsawoisx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3kskxwvbz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3tdnmbbnc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3maegarzs.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3sabxslyh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rzprymrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exxarabp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3odfqwhna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwmfrxci.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3snmequel.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fbfrsivu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3drujnick.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3agymkgcx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3zofpnvgy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tajfbmmf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3idjbfcnr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3qyizsipb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hdyevoxa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fvygcnix.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pdwiwrys.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fcwicxnq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lzmsouiu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mrmlbdda.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lbtiunyz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zbrdvmjb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3gwqtbjjv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3lrfzoyeg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qpkfrexg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bxsmmbfl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ubsvadbx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3zknaqyft.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3brhpyhyb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3spkjkfng.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ypmmckak.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hnhbkxdo.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3begegzoy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bmwzpvxt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ugpuyyjn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3rqvzcfok.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bxdwyblm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pqiljdbt.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ikimcxoh.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ihkkcfpu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lwzfqacx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3iutbnldz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gslmlygi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3oujojxel.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3vgdtglxg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xakuypac.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lwooacki.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3iwzrdfoe.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3nvaxkgri.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3rxgnpjdf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wrougcbc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3psjktpee.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cxlijodl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nmezkwim.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3buqyjuwl.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3itlbqmkk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3iswzfnvz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3topvhzln.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hzduhvie.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3krtlmgfw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3cdrprtdq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3bkjpuxtk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3mpxtlmrz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3okbasytl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3xyzwlxjd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3lhgzgsst.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bitwqjte.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gcbjfjmh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3smkfrrca.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xnkduynf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tcdpmvhk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ouwutbgl.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3gvlagsdy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3pcfhumbj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3byapxylw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3woyxvmof.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ciefebcd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3cndfqruf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3tbviyluw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3vrpfdcqo.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3hfrztzjx.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3mgwcnzrh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xssemuhi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3agytxlpg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3pziflbgz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3azomwbay.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ajzkbhcm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jtuurngi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3uliqdvou.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xuxhbzhi.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iczgtckp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3gzueyiaj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3sgbrosqv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3hsugsfag.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3bloajukz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyjnglmd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fpctkbzf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3snbiunzr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3cryodjgf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3awcqwpls.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vdpkwoyq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3hpaixgem.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3auickmrs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3phcjlpxt.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3eptzbvmd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3xnlumpcg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwtixehc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wmwwigly.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ufkpipvu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3bwlvhouy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3pmoythfn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ybmoerkb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mqltbfrn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ozibhrvy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nisncbpm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hmctfncd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3xqjvkytm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ovrmyesh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3eljxpilq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rltqdlra.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vmmmpnka.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zwjjmnty.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ruexhhul.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ttjxqngs.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vbgayqrb.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3biuqmnex.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3nbmvckjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edasnxsl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zylocsgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqxvwcxu.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3jizbmyvn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ntvlqoja.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3auerhsti.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vujfccxv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jvlqwceq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zgbupcph.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3soxdyvsw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3czsnclan.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ftxackwz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fukhbuyk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ftdqhesu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3dwsyhvvz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3cihjijps.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fhqwausx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3gjngxscq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3hqobfigw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3jjzcgnmc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3pqkhfuqu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ncgajgid.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3cgraxvbr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jayquvjb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3zgsufuvk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3vfpxtjun.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3umekjuru.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3uneejfoc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3lvptgefu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3nzzaazoo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3xjmptwrv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3xummjxkz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3vdkzkumm.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3xabwtzaf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ohjzkfil.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3avatvsfx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3zdvjqgcp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3baezddvj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3idkqphwp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3mdltmvdp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3mqzrkebn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ayfiaepp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3kpspchol.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hooznpzh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3bzvidxby.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3agaszcij.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3smysldod.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3rlupzbqc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3fearsxkf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3mjwziarh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jnsoqgqy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3epyyxucz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ocukpmwr.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3gkfdcyqp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ufmwrrrw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qogxzphx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3aqoeugxh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3bamvsyxh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3oedddgwq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3omykgrzi.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3vutdzcwn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3mehnfgic.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qwkkiwio.html


<!-- 参考信息 -->