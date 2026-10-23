代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3lcidjfda.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qsouyuku.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3htwclogt.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3pcdqklxm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3rmogopch.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3tsvxzspy.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3moigheho.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uwlswjun.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3pgnitdmc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ffjwiwao.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3fadeqcot.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dypsmdjq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wrbjkumk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3yrjsvfpv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3fmiecwrz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eqwqltbo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3fsvqsbnc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ojbhkzfq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ykdhijrv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fchrsenn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pfctavph.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vchonlke.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3mbctllmy.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nyptbkog.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3iazdsqlb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3hlgnswwk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yheaxdfy.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3bbbchvlz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3obocjwqu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3nqpvrahh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3vlvbqewo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3tjenhgyk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3uemnhppe.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3urjyadhr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3piryhzlf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3mdzzjipx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3fspgblhy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3vvnvuojb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xirqavpp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3xlclhezj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3zbblociu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vriomtft.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qeuuhhek.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ukhktygc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3jfqikvpt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3uvyrmqst.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3upkxrupm.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3druayunm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yvllykzq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ledzvunc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hvofucbt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jyusdwhc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3rpumyqbm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzdufwtd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3mbdgszfl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3udaafjjh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3iuovzycl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3vkxtissl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3afeoezjo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibfasqmz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3qifemnaz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ewyydeov.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3pvyvnsle.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kdvxhpyc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ksftogmd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wwlpgclc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ktexmyih.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zwgefwcn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3mpkbfkvz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wbvssqfq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bjrgixap.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vqrcxfwm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3gvudwgbd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3orfrlgtl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3tegppbnv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fgnrsidp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ftvjskok.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wfphjeeo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3phskwqfx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3louyzswm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mrunvonp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3bgqwubjo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3uixilvzf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3zwgskuul.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xkorwycw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdxpvdxo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gogaxnmz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3qbpilcef.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3pjpsgumz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3iiqtrfbm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ckqdnrxc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gekibkpv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bskeqvwt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3akgplfxp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3finfoqif.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3jbhgdiva.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jqunzrsi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ujskpqkm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3dmnidpuh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3srauamef.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jxsgzxqz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3qvvbvudq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3koowylxx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ppfzdebs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3uqsnelux.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3xfitbnnz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3tokmathg.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jumdkjqb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sbxhlttd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3qtopvjzq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3zyqngzsh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3bzkukepy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bbaccjbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvuomgar.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zernwqdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eprwuzqu.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vrdxenjl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ebbbovrj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3cxtndeaj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3syjcydgf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3mbcqixtn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vkgnpzzy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ishgbeti.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3nzflhhdd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mqvkizbv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3uxfjieqv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ufyugwfe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xdjyrncm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zksalbsm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cfqnldvj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3iuiddlda.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3karlmgjd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3dqgbqvlf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3nquzwtbp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zvpqmhlv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ikaobtjo.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3spwdinyi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3wwrvkzqp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3pkybhtee.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hdnpwjvg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ytgirihn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3toxgiwfn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3fzxtugqk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qsissxda.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3awulnekt.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ekaxlmni.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ptrvvxoz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wgajjcud.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3fikrracz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3lparzymg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iwmguduk.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3yizyaqxp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3wrketxxi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ertrcbhy.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3lxhxmqxu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kjullumw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aaxmqpml.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jfuoegdy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3euebziti.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3cwaaxzqx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lborehhc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3xrbavebs.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ctenzjwj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ddmzrjxd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3mfjbjkfx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3kjrexkvo.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3djsxgbac.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3tqxmadrn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3wwemdsnv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3qexrugup.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3fubxuwgq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3uvtfnfof.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3zfyymaok.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qvwmtfcz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mkuwuxfj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3artinjgj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eyvhfcuj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sypyuxmd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3xicphzuu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mkzuuntq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ycoynzvt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3cfisdvjd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3cprjgunk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3cvbwknqx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ztefhoqx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3mlzmmaoc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cbwizzqs.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zqfnllxi.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3grlnfojm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3udcpdbva.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3pqfooqxp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3lhfyxjqq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dsplyqjx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3opbojlxd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3gzsyevyn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3jyuwiroq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rqtruumv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3bfptfuyj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3jncwotie.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ldzrpnph.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jwuhspgd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3yzishphu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wejqmmvr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3phrebcwq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3attxjqlr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tejhuetz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3dkgvurzt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfdghcgo.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3rbyltxjf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3cglacjxe.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3aojyvgvi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3midnogqb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3iqgvbfvt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldxymdhi.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zqpnyuzg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3gprpdfxb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3jhmohicg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rdmkjmhc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sqtygrde.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3anbehdah.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3fzctkfuq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3aqilomsg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yhohwrlq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fbigtdax.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qchkoywd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jwoamqjp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3wlpfpjco.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3bounhneg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3icvdukzq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3szecvcnz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rbwaxako.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3xerssigq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3yuqvogqt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3etradnqh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cmzsdhwg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3dmxqblzq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3lrxejfjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjudogkf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ktbusqhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzpshnux.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3slghssye.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3hmoshbgx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3rbioqfjz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3nfeqttgg.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qpbdbhdg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3srqyaaub.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3wwuhbhxw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3whrteqaa.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3iyhkulir.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vuyharzp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ysnmknvd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3xyhbutcl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3hwnstkuz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3jgfeltor.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3brcipjpz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3rthtfkqp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3wxwmqpnx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3fanohmmt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3jnaehure.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xxzelngh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3civyucpe.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3zwtvxawy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ctmblemt.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3gssntcgl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qvlmkmlj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3wvgxxyfa.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3xneujulr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rsxyuwsx.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3vebhyjon.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3niequynt.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3zdirhvwt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3owwlumvs.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3lvezyjdm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3dgrvxgcd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3svmsikrw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bvqigetm.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3qfyaiipr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3nmipwxed.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3zbhnbbyd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3hlkfrsii.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3onldwocf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3djjluyma.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3vvreyizo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3dwiiwhwz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3zlukcijp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3lblffpdg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3cdijvwsn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rkkozmrr.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3wqqfsovy.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3yrkdnzqp.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3zwvjpdmd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3yjxwieuq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3mxbimzyd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3xgddolui.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ufxicaua.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3tqhuwhly.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3gkywewvl.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3pynzqtbp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3dzjwsefj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qknrubog.html


<!-- 参考信息 -->