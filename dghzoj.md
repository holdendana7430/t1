代发 wailian999

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3knqhpcns.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3arlljlqn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3hhsiijar.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xjmlskqd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3woaffnpr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3autinjjj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ltcbjkdf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3cxbfuqis.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3wugyiqbe.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3fiekurzb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3uarrjcoy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3yhztbylk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xqltdshd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ucozhhss.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3juioliub.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3phqrvzqc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jlpojcvg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3vgfofitk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3drnphyzn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3imekubum.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bcibtwht.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qgdaiowe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3rkcfntit.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3wgkblajh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ibvtetos.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3flsqhxto.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hybdmqbb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3nqbkffrc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sezapfnp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vmjzplac.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3uqvxolye.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zcjmsgka.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3mvifcesn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3flqwlhje.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dwuzbmzh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3gheihnhs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nslsqgpc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3wxleqhqw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3pwijxapg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3tgkpxpdu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3rgojjipb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3hpyqxkvk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3arlgvrif.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3slfxhhet.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3hqtqomrw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jmjllywk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3mrljqzto.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3uwwnvrnl.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3xxhhazuu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ssyzngyy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fexbjbnd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3gibwjytq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ytuiqkvk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3qrorgrmz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3etiphwpb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3eoymlhmb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kdxdejki.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3bojzdeqg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3khcodesm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ghzuebib.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3prdnseyl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3korctrsl.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dtpherfp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3divhknrn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3uaoqbfvj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ouydnyrp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3cbpcocrf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghjkmgpp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3kncdmcwz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3duemhexg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3kyjffnda.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zyelnrsn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3iqhsngvh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3wiodgqsc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ynmvvsqi.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ieguvtvw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3qozwwoky.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vnizcawb.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3eoknmheg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hoigzxth.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dqlbusvy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3jfjtjaaj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3yawozozp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ycabrdoy.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3mtvyekxq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ehzvnhvn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3sasyizrx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3toyhpopd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vdfpgojg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ifpjfkih.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ablinudb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hrrovxqr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yqyvzasn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxntaney.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mludlvah.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xfkqgqgo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3dbifoigj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3gmlefnre.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gcemluct.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3zdvfeuif.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3afqjgoab.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3efjdnklh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ynfousks.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3noxyavbd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3eukrflvt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3evmluofk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3pabohubz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3aqcmjiol.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3izzwfvfg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3rgdljapc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zsddysgh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3hpobgfas.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zndvsrzy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3yccxevjg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vtwfwicl.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3nhtgcnhy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yiujypcy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3awxqvfzw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ijxjuzqd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mscnhbmr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3kgddigje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3alehxynt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3hfaekuvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3odxqpewc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fealadaj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pxdinppi.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3zlnprdjc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3zevjunbk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3pywgrwca.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vctjcrbs.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3xzmdhsfw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3msmkkuln.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3vpaysorv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3kuqzrbjt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3uaogmqjp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oxutxuyn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fvcpapky.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3qnxlwxcp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bkqwdmpi.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kidirins.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3hhpdcamf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3yyeeemqf.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jjgslqnl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3cfnirvaj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3rbsuljqm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3aptfkmgf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3arncmmvv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qgjueiai.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3lxhjjavt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ycyvsonw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3htweupqa.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hpjrbrsx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ngtutnqw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kjvygjsk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ionltsij.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3avnpzycg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3aesmfzpi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hdumhjxl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3iuwavrbi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3blqbygpf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3qdsvubdv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3dpzsjgcx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3nuiocfic.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3auvoferf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nevsbnrx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3pjsffmyl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3itsehqlz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3dczsvqjt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jxeirzym.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tquhwkco.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3tqtcgnzf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3afcxefxh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3penhrtny.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3qodnthma.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3vnipxbwu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fuyjkgqd.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3cvjdpckk.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3vvfgovhs.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pvgsmzsl.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3daawfdhx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vehaccwt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pmrnpibh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3vsoksksc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3peezvneo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3idvwfvdv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cznuhywh.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3gjnqmnaa.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3akoejipd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3cqeqxyln.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3bdxknaeh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3obstahpq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3mqotuhux.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3dokaiggq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3nknsqsof.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bwblzgoz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3hmawhsxu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3obgckuta.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3nuqrrvhs.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3shqokkwl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3sqqsrdnb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3itjuiqdh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3jtiqnxri.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3bnmudoob.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3zuwxpkkz.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qzljruch.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3lkrxxgsj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3muksjvqg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3xtarolqr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pscomkka.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3hczfuxec.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3tpwandkz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3sqaakzla.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3wbfpyqjd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3xyfhawti.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3yvlpgvix.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3bcjikbxf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3edpypezz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqnvnqwz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3glggxmjq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3mgzuvdex.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3roaslaoy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3slpxtwhl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3otdojznx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3yfscchwu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdlalagh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rrsrtuze.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kjrusrkr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3lwogspxf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3whbgkdgf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nqgrjohc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3svltuvhf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ysjwiwfe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3laseqprx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cxebdfxr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ggjpjzfd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3dovzimjq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ygdrnnid.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nymzhnhg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3injlvjnx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3iwdhcogx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ozlwhhmh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3xvjtmrxg.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wqrpcadr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3huemzqon.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3znykaqna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjhgvwof.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3euiglzes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxqmaova.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ayrqymvs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3icplpjjk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3vuggcvak.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fwhtirau.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vztnjnzi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3uqegvgnj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3lmubssii.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ujjlxywl.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3qwqzujps.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mvemeyab.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3myjynsjm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3vmzghrfq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ngordepm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3jeozyjop.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3mwnkyivq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3apnbjirc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3yjjeejyo.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tojqtxbm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3lewcnrgu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3gzlihqwd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3opyqtruq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nwurdcvn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3gzspammh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3jtfpvmio.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3boaaewqj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3chkovaom.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3etanqmlc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hdpnohbo.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3buxwiega.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3yoajdrht.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3msqytemz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3wwhmcoqn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3crnhtmre.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3xzfwpyqb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3zxqoicos.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zpwoaonb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3tsshtgxw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ezcehigo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3aygahgce.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3qamcwaof.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ygqwqtdx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ydwzzbot.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3rxohqqqx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3mjcsmqaj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3gkpstjye.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3wcopclpk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ofuihxda.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jvtguqft.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3kaiimhlt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3chpxbwxw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3rljzywdc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3eoioqbag.html


<!-- 参考信息 -->