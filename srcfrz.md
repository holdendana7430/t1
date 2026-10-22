代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2dawsgwgz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2vljlvpsh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2aeupcxgt.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2pyprqivl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qbrgbohh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2xrjjuido.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2uchlolox.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vqdtaqrq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ftpslnhc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vyqwciwm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2uonxlqki.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2vpgnbkaz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2tagypreo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2uuofnpil.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vrpxitje.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2znefxshe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2naeynaxv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2mluuluxj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2brbfwfoy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ejvhkcju.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2yqomlakc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vyknpdbo.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ceaueszn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kvivaeqc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nanvfcwk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2bzgrjbiv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2qostgzqj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ntasokiu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2tvbwbajv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2mafyufeq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2iowplcdi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2cfdzcuta.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dcjntemj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hygvrvcb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2cttedwpk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2kxilpgsu.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2iqkrsuue.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2gdxrahty.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bzdymacw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wiiiooxk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ynuyuuer.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ghcflsdt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2rejklgvq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ejbctwix.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2xhwodqim.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rsqauaiu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ouqjdnpd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2xhmqszui.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2gbxwwumf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vmgiscat.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2rmgpgrcy.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2cmkdytdz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2wawsehqg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2czjpliqe.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tucabbkh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2nnyjsnax.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hmuhmbak.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bldvvbvq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gioiengb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2znjhjlux.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hxxesueg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nlflrycw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2whmxnzuw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lhodtzyx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2qebxjnhz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2djsukbyv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qdjnvisc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2dunjabgq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ocnanpaf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2pcbemtwl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2aqfuhcel.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2gwqzxexq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mwvoamqk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2urkjlkfk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2czndfgar.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hbgurgwy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2mahhwbrm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2inlyskht.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2rzaxmxhx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jgczodmo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2siiqmatf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2avrmfbev.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2qaosmfhe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2mpnlbmuo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2jleediht.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2czrvtwhc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2symgyfge.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ciairqvb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2sxugdslo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2coghxvyf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2emqyfqeo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2efawcpwe.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2adqmkptb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2iebklqni.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ntgjwlmm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2rcggddhf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xjxjvrsl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvcohrtu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kdcvyhpt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2hcprzevj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xifpduix.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ihgdtxyo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2sdkwqquo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2wipsotbj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jxqjxnfh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dixnmhzg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2fuwwatuq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2wfeahfue.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2erslvuvb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2hpxaludv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2xjetcmii.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2aekdaysb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qlpnwuqi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yyhwftai.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2umkfzvuf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2rvhhllhi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfrctlwd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2oabgajnk.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ntjdneqv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2fnyeothx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gicpgimm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2tfrdjpoo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2abrxsbri.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2uytkxmkz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xmewngjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxiyghha.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2oycqnrlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qszyszeb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mezfzizx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cingsyyw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2esgeimtd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2vdixwarl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2snjypekv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kwqamnnm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ohgjyaxo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2plqcsqie.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2aohqtxwu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2xvdzvzay.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2uqmtjjlw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bbumsdqz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2yixltzrd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2diraglqn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2bvnxrlay.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wropajvq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2sugezugt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2vtmwegdy.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2zmclolea.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jojdgzxh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qdnezbzx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ywdseman.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2iaqecrzd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pyvwjskg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xfahyqrc.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2uichnqzl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2bwnxtufu.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hwapqsdd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2unjjqpek.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hlznfpwx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hoekohub.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2slcjkofu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2mzwpubly.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fhwisyyg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bhczhqsj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2gizkjiaf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rzooxaso.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2rmvtfjip.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ylvczcfi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2pyisduru.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fpzccisv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2drwctjgv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2vtciikxk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lpuorsex.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2gbiopgmu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wcbztllt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bnbmfshr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2etegqwzo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2dazdbiun.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2jqdpzuho.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2yhvwvlnl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2tmaeilmf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qyclxuaa.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2iekwgxyb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xqmuffrr.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2nnkvlilc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2zpnkmrpc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2pxhvkrtk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2mryrvyrv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2tocpefuq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iuaijlco.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zvtzoski.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2odtxbzsc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xgwftofo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nvptbdem.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2eymkjahk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2yqyaxqux.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2wwqxpjfu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rlszursf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bxwrcwov.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2sntspxyx.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2jkovhcgb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2szmbcaid.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2cyxxryso.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2grumpdan.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2whqxadkb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kftbfnnt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ijwysvyq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2byjiwhcw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2oqwixbwy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yeqchzju.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2tqzgpysx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rlfeanut.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dacfekkm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2emjnpfzc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2pekobucq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rlxtvyri.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmyikrpr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gbywyhex.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2jsjkpbnd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2xckpmdpa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rearjxks.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2xkpmtbrf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2dakeeeur.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2iudgpvlg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2pxyrykhv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2mjuzwajv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2falgislp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zmflfeqy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2uaapwyha.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2knwhykze.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mpeyjfhs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yplkpccl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2yocdlkot.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jmhuvyhl.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hwnsvade.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gwgcnrkd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tezvmvvp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2savwckyi.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fcpbdssx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ushhnpuy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2icwdciov.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xhdqtkhb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ikvryqdh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ehlbdnpa.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2pllniukd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2nteyuqxg.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2jeyrokmv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2aejxaecg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2fhwdvrgv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ipsppzae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uuvutlmq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2btvvkbsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugzgmyss.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2zusuycau.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ryrscrry.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2bfvflszz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xgoxfjib.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2chfbndtk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2lambuopa.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2etgixtvd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2xbatephx.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2pvhckvzw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tcquutfr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2rvlsuztb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2efmhafzk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ryiwfmfu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2cccgsyou.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2aplilqsp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2dvielpdo.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2nnrqfrub.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2xaojnjdd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2zospttgv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2yriqmtoq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2lgzgwvqc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2rphiesaf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2uesssaat.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2cifybvdr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ctaxkljv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2cvcnsozm.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2aljhlqaw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2cffuayip.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2sofegfaz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2wfokqtii.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2qdialbrt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2tioydxmc.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2jcskdcbp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2cntxypas.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2febjwsow.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nleeszef.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2osrdydih.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2pxyrktab.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2gsyvnwby.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2bizuguyx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2llzqgpna.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qdpnqjfp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2xskrfroa.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2mcbbvxcb.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hhpepama.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2wpgeygyf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2jverargr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qjyhqkis.html


<!-- 参考信息 -->