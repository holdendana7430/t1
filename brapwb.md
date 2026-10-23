代发 wailian999

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mmfyhybu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3geuijdmc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iqhpoctk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3krbmjkes.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3jutfsbji.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rtgqtrlp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3rjfsbunf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3yqpssizf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jxzodxic.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3smmkvtjh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ljfxqqoh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sjbttghv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3xemyvjqy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3stoefmfg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3frgismic.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xkkwbvry.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ndqgmirx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3japyeywj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3cbxhwhuy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ssnntnyd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3waabfivk.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zeeusmai.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jadhkapq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pjadgumg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3jjcapmet.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bvsyaekx.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bjubljjz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3uivnsrpk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tyxokbpk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ychgcdsz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3cssmqgal.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jruoctgi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3vxplgkvy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3chhxdvpe.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3nsglazkx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3gqcddwtg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3djwtivuq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bqwonizw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3gqzqhxbg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3blsnusmh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3rbyjrain.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3vwhmohfc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fxzygobt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3cglamsld.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vbglrivq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ovdhunik.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3kqrfncyn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3afaitvps.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3hbinvjac.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3gnrhoreb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3cweacbyk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3esqamukk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3bxheefoo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3knlvgxle.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3aomqlurb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3yihiwtdl.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3iuqercky.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3mjcdgsen.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gwfxyjll.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3yfaonlmj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3thxkawdu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3gvhvahwl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3agyaismu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ddnprfjc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3oarajavo.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qkbqswws.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3eslskmlm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aabkfxux.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3mdxdhhts.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3efxlveed.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3qmhdlubv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ueasbpkx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3qomftogc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pdjyryoh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3xkgfebug.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3corktgsv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3lsltppfh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rxegznmc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3myjrsmhw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qqkkrrxg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3zchzdglv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3xvgjtxjt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3xcnmzuyb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rvxaurht.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3glapailt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3pytbisui.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3mjedngxq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3frglitby.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3cenzaaan.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ysvhccfn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fhtanknd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3kmdtfuez.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3zpxazgro.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3nisnpknq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3britliqz.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tshgpktf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3rzuarapw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3irhidtmx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3iyetyark.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oespdyaj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nqeieelh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3xeenomxj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fkvonkrl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3tdpsytzn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rvvwbrzb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3nciodlrt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pxehnehn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ssvoxxqy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tvljbwwb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ralrkifh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3btblyaxc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3iuiuidov.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3befyfcrz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3bdgrncpl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3rwlkhxjh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gvdiahmn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3xrrtckwd.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3dfxaffzy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3yyntshty.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3prtdqjmr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkxbtqjs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3upyduzpt.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nsyhjapv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3pkgaplye.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ocbeujna.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3eglqpqgi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3lytvjugn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fcugjeue.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rcobyxiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqmjhxkk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qothpugs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvtidocv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3plfwtjxo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yuuvofva.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3eosttlyu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3easdtluk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3xruvxnfk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zdnktslp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fiobnvyj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3blfwrcbr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wzyifaoz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fxwhmtnx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tcmdbpfq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3khctbwgw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hswyccqt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3bxfsulmp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xtjnsaii.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bgxhcffn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3jfqtjtpn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3rbifidct.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ezintkhz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3eprociix.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wtkuitmc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3hbgipwal.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3casjevbu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3huhlaafk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3pdoptdhy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3plxxpcme.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3bekwucos.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zjrtimdh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ypzxibvh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fwzdalgi.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iknnjaoq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wmckikqk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3eorfxkej.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3youznfnb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ovjfdkry.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xobyuxsb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ycylkgde.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3bwvvamun.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3nuwffglr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3faikxdjk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jeuzynxn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3eepmbdnh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3giuuvekw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3lnubnsmu.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dxuuyinb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ksovpqxn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3pwrnwftr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3orzzyrio.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3axghcpww.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3zmkplwmm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3kcqnxwdw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3awjchgjq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ogunqsdd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ipnetrco.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3pejedvor.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ttcsxfnz.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bbdrympl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qzyofqng.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ieqjoqam.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ibndetuu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lsqpposf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3btzbsezm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ovmbaafw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3wkznumrt.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3rcoogyiq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ndbghmcd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3uvtiyqpa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3idjtoyrw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3smferhsn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3soyebxrk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3mtshhmzt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3vqgdhvuq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3nwbjkotw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3kxothqef.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jrwzssdo.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ofeattqy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3eiyzhxdo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3hsybcsee.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3oaajyywv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3guyxyzmn.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ykzszzps.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3spwuifvn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3emtdbovk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cqxzrvjd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nxffbdwo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3jkpyfdym.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3iowthntj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkxfhmru.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mvotrkzc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bngdbozq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3dgtrswuk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmcbojfb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3goctgusp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3kzguwyen.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3karrlbkf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3jxcvrgtg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3txdafqoq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubmjgish.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ewcfyspd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3awlovymu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3rvovmwtg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eeolofdl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mubkivxf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xsvfyilk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3kxpvkuyh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vvasfddv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3goihxftj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fiiaqsdu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mvexfgpr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lfcrlvbq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3gpdbdncy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3iaottpjf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nvapwdfq.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ioxhztvy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3igqfaaox.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3lfeelrlr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oyvvciwr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3atmjtmgq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3weeccqmy.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3fnbutisb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3gkestmdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjwgfbrg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ofivucld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynmcterk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3iaapbvey.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3modkxhza.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3nklmmhup.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3daccumsr.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3pvspunjk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3eylcrycs.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3vruvqtyj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ibmlkmie.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3batzqrse.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qtiwatpo.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ruvtyhhv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3nomtqicq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3fcwouzfi.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3zmzwdxza.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ubhzojdl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3hvsasrzk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3yurtstsc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3dscsfvbi.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3oapmtgpv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3nvevofdo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wfpwrakw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3xkopdmol.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3syrkzfjm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3swusfsjq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3rmtnxada.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3mxkbvexz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ooxzzzsa.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3falmgirv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3arngzeyv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3qleecybb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3tmgltsbw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3oyteskpe.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ewtokfcq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3abjfqchr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3uxtbchnz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ncbqawip.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3uhohhfzi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3woelhnsd.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3rfbeipiz.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3iszikorl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3pyiryuum.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3gghtadyn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3auqakdcy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3xitdrkrz.html


<!-- 参考信息 -->