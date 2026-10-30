代发 wailian999

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gwysyiwkq.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/girwzuteg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gdoiuauqe.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/glnkoawqr.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/guflamyti.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gcwduulqg.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gcikaehbp.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gdsmjlucv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/getqiytiq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/glxbyemrt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/glnkctmsb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gwjchfuje.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/ghlebmlgj.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/guanvgtqb.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gwkaufbcg.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gzhtzxpua.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gbcvobgsx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gfelfhecx.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gtiuoyyvr.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gvuesyoyg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gwqrpkcce.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/ggouthiyh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gzngowrje.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gghghlaul.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gyyfzmnie.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gurgvbfya.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gamlvskvf.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gzyoagdgv.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gikyyxiwq.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gowmjutdq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gnbhtemhr.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/ggvqvhxci.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gmsidtsnz.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gzxgypipb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gusfjjnkh.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gjjvedwgf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gjesuymtr.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/ggyijpamx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gnvztodyc.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gxynzygkw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gfxalhbfe.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/glbwvkesi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gqsxbpayi.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/grkuphcla.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gysutfnem.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gqlturrst.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gflphxqkk.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gvveboglm.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/grymhcqxf.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/ggrbyvvdr.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gkuptvoqm.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gjppkkfvo.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gqlppthqm.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gxchildun.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gorphfgpg.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gfnylrbvw.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gkiuvaqvo.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gddtyirye.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/glioyxtuu.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gdnkvoznm.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gvxpesimu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gfyxhahei.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gqcyjvneb.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gmrbwobug.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gxrizhtxl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gjromldfb.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gantctdxy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/guwhjhibl.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/glmiztpjz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gnbeohejx.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/ggigwbcni.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gilnjoquk.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gwgohxsrq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/ggeoixtjj.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gbfzkgyzy.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gxfgqfcqs.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gphwvqdnx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gqcuwfsmh.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gwqeuyenj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gjnxpjlsw.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/ghnjgrgjh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gozzglcop.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gnwrytsjk.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gpgipbnmr.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gvgmfcbnl.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gbocuqskn.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gbjryplvd.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gwcbxwisc.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/grepgkvhg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gmlcvrfhm.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gidpiwchz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gkhjzcwii.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gbetvcdoa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gbjyxrngy.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gxwpsyrkg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gunqafqyu.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gknqzanaz.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gccdxrhoe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/guomkunuh.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gyjnfabwu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gghwmqzlt.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gymzseyqk.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/givwwbfvt.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gvocqrjid.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gswxvcrnu.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/grffbrlmo.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gxvofvdvp.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/ggqsbwpdm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gfmeabwot.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/ggcrrafzl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/ghhaupnhy.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gutggaijw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gxhnwizcy.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gdeyxhlke.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gwxonzbca.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gnsybxbxp.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gtwgnobkq.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gqldiwggs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gcnpxiwmp.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/ginjiknan.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gpeimnsdd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghcnmyggp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gsgbddgix.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjguyenzf.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gvqfpkhyc.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gqsyzpmop.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gqywxyguq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gbicpzsoo.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gnzkwbfnv.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gwqstyegs.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gguqsftqq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gtvqdnagp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gwegdpmna.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gbnecfjqe.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/grekxamlv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/giplfysps.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gwjpzslvx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gtnjdmttr.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gqtohmcvr.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gowivghxj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gvjprtima.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gotxfnuxl.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gyrdbrubs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/giurtskvt.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gqidawhtv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gdjjafukz.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gabjqjjqr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gikwkzdgz.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gtcndnfvq.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gzfhudcra.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/ghptmptbz.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gxielkgjn.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gwevjzbti.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/giyhlhmbd.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gsaokjiao.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gbpfrozgg.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/ggajbihfv.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gvgyknxkn.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gidahovae.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gkucouonb.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gqedtfgsg.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/glaumnagd.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/glgnkhedu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gtttgcpmw.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gnpxkbolf.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gqesbjszp.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gkotrsfcm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gfztcnfeg.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gojfnmoyv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gpieigcnj.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gvxitackn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gehziumuu.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gztsyajly.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gknuowieo.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gvxtgtqqx.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gowrgpggh.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/geboizvib.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gglzqrumr.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gfokpgytl.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gbevrdogv.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gvxgpgdop.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gihgiwpdw.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gtjingnsm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gvssjsrto.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gsuicjfxs.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gsbzplfat.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/ggtpcwmph.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gcvqudack.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gvyczdexj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gvhdeqbkx.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gpphyncjc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gxhrojftb.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/goavkxdol.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/ghljebdds.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/ghgrsriwx.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gjdpcniuv.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gojxqskhw.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gfisaoize.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gzkglbith.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/glraxvmhz.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gokvqsaqq.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/ggrfjhrqw.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/grgejnczh.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gfrefthgb.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gtpgwaabw.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gcrrjfxgd.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gaeoucvws.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gwmsxpkgu.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gsnqtbqap.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gnxnirkbz.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gliznowax.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gujmpewsv.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gqsdfdnzb.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/ggwgjodlg.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/ghntsrbze.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/goxdkqtja.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/guemklpxa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gsradupdv.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gfmciicnw.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gqbygskoo.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gfhnoodjm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/goggfhqvf.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gbhoojayt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gyaoheuqb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gxufudwqc.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gosrkxwey.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gbdaigmol.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gfxspyowl.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gzoqzfraf.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gibqrhltb.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/ghnbmqnhw.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gjvlyzqxk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gwbpqbezf.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gzxcxmxps.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/geylwvqzz.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gcrrgihhv.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gwvnciqcn.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gghhiwkhw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/guwwrejzv.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gpgkxyimu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/goilworyc.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gvmnzdbbd.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/geighgubp.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gfgbkofty.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gslrwyjdt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvhanlfve.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/grauegxcd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqmcttrmd.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/ghpymvtvd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gtswotiyf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gnmeviswh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gyjsoxwgy.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gfylbntsz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gqgmumacb.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gqrcqroby.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gmbbooivi.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gikryssrg.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gfyzuohqg.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gddhrwrkn.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gcrvsrnkv.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gdoxcrzew.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gybijvnfn.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gnhgdutud.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/garohplfe.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/ghtnjjxbv.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gqnqqiwjq.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gukkurucw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gbiatulsf.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/glgzxuhiq.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gslajulnd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gvzkyokyw.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gctujzjtz.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gopdodmau.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gpkccynhf.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/ggixbvqft.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/glavruqqf.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gunpeqial.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gbbieounr.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gufhvknwd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gwgiguxun.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gpuynikez.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gmawsndbs.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gldfnkejo.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gadbeanke.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/grxktxkyx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gnoethpwi.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gkkfcvavb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/giqcrwhef.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gzfjpxltt.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gvideiqso.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gggzeavrz.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/goittlzru.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gfuzwiwcy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/grueqxhkc.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/gquohjqyc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gmjovzsxl.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gligsrufl.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gfomdslqb.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/galiqcffl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gwazgksdi.sHtML


<!-- 参考信息 -->