代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjmdqiph.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ovdwwagt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3qrzflrtm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3cfjuxlhz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3matiagvy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3tmhnnepo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3eollmrgv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qteqhpqq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3abhxgmop.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pbkhisik.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3kuoftbft.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3xhlyewfh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3fxrfqpmu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3tqofrrig.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3nqcyadjk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ycfgkpox.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3dyocqpsj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ynbkfigg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3lbfduwdh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jfscgacy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dnqekldl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lpkvvudv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yxyofpyd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3fwjelikp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3glmbwxwc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3yulzcrie.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3kohwrdow.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vtsmkoqo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3pgbcfoyg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3mavhvfgz.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xzvjlvst.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hkwuqqtd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rldyasgn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wvwzwrrm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rilsznxu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3cemclchm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3mxxooppk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3tsnsrpuo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xbdzgjnn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3jxvwvlht.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mnltxdpg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3pmslybjh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3oppuauif.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3nmfobcrh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3gazglres.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3xcypbnwc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ctyewzgd.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3pucptwme.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3qbbutjns.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3lzvaskuj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ugawmuvz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3vriwyfsc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fiuimbqn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3xzrimamk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dybmwxfv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3juxexwng.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vfyisyqa.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3crtorbta.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3eaqyfhss.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3lsdfktkn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3pteqsovg.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3kngdgxgh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jdgwbibs.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pnrxwcvy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3gztdudfz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3glhyspno.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3swyxdlxl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3tqogagmh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3gyuztdbi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ehrzjcpg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3glozpfoa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqypkqmt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3lwzjgvoo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kdpcqiim.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3uiqozdmi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3phetgsbs.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3nzqmennc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3geitexcn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fytacyhd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qxaaswyw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3mohietvg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3brjiqdwh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3fbnmwsza.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3kpdaccsv.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3sxefwzrz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3bpkvunym.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3tahomunv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fpluwinx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ybgbbnvy.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3dijxbwkz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3fyzdluqm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3nmnxdmjr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3gvpktsry.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ticncjmz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3hqmamcva.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3mjqaynls.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zuevpmlm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3xagnihwa.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dtugmorh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3cvsgiqys.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3lnufnnhq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3iqgpkwem.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kgxfmclx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3pkjuuiuj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zsqxurka.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3rywctzov.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ugtekwyk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3xklpytss.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgcxalop.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3gnktmvck.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3jtxyttrg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3wbxznmlj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ndsjodds.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mmjmmlnm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3okypzcyc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3altpchdu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3jxmuarpt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3toqgpeuz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3knsdzvqp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3budydlju.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3phyllafg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3tbfktrbj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ibtlfbrn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3orsxtyox.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sjrlnlti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uyaittcy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3fhthkdnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jejphfxv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jmzwjlvr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rglayuss.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3asrtmezo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3cnrywnvh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vunvwpjd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3thkeqmrc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3geeewofz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3bxfuioqm.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3xtftdrix.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ponewqbw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nehehuhc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3clxosuob.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tkjiphzn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3skgyjcvo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3vtnzewsg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jbocblvn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ccaenyqi.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3jjrnbnnt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3yztbpowv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3bgbtpgkd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3kumrjvpg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3anqphems.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3bbkbbyrk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pljvnqnu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qahnksvf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3dkmeaxcr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ldhmsvrg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zhotsunc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3denbxawv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lgywmgdt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3djpcdrhk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pmdkjsrx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3lckzvvpm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vtahclig.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eahqihuh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3kjpqtuxa.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3mayqlyff.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3lagyimhf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3svbtsvaa.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3yakejdhv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3njznrqus.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3utanzpvj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3epnelimx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3qguzkhdr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lvyyqkyn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ncxqqglr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xfhalvqb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xwifltsc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3kmnpajdz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ndfjyurp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3vouxygjk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3swbczbta.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lzcfrtza.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3omckioic.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3hqoezqkl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3zuakhcwy.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ipcwjaqr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3qjwvqvtp.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3nykxkdxj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3rbmdwlyr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jixkjdqm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eamozrnx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3irdgiibf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ajcrzawz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3wyybwlsp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3rkplgcvm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3zmzfjhga.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3mevrhdvf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ezdyktzd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3clbjoptf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3shrscoub.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3drydbgtz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jevjybky.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3hdmqkkoi.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3mnpdbfud.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3pngvadjo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dgyezfkx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3aeardvsm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ryqcctgc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3kmdppgyo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yigkseig.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3udkjwmas.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wrykjukh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ldzjpkze.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3oisehuqo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lweaaoqz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3inuayuch.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3mlogyqwn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3qfwbusix.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ctsqpkay.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3suypwijz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfcvbxiy.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3lvsmraot.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3tyucqjat.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3iveohdcs.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3eucobjbb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rrivtqvm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfmotnkf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3odmasdec.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3udvoczrd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykohqidf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tkyxcupk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oebcgqnl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3vjkyxrjl.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gicdcdze.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ovhkmasw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rmtthurh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3prkjshev.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gpwasgjv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3twmosedm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ossudnov.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xkpaelug.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qqpkcecc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yrxuwkuz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ongjwvhv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3garkvzam.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oucubnak.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3oxluqhxg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mnkcoujl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3hfsobwqx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3uluifawi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nssxkyck.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3iptkaiaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhjpisbn.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3xopxsxng.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ofoxmjfu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3pdihbtsd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mexelupl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3gihzbcld.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3opctwwax.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ymcbtbxp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ycdkubtb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3azvwqrmx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xzmvlxbp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3udtcxwco.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3qhkjkkzx.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3crevsepn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3eqovulln.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3foajpqxw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3yzryhmhw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3mkfvaiid.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3abevqomy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3jcxrybqf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3bpkxnqhw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3atsuitgj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3uaamhgpw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3kbwczqdn.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zxdtuadz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3bswlxoyn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3mtskojjc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3odguffgm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3foekhliw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3odksruux.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3jtmjtrlt.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ilcgndvn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ptptkmti.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ifccgpvf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3jlbaajjp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3plwyfisq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gmxqkemo.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3cnfhouyz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3pzjsvmoz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3hvuizfjn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3feytlezp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3kcwgamru.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3sxyyzsbt.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3dlqmwjpv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3fszceiww.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwkstuwk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3slxyshyk.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3yddzgzgx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dthusrfn.html


<!-- 参考信息 -->