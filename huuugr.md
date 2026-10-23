代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3trfpcquw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3dpgshpby.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3jjmuncnt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3geyhccwf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3blpmqlja.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3xjpmyvgg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kplnyovn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zprsnwmx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3hhdedumr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zhjrtorl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3nehoilsd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3zxvedbvz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3helnyetr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3tdoufeae.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3cthopxmf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3hdmznwxh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3aitagtom.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3wqfzmfrf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3jxosyyci.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ikaopyjm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dcyvbqra.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3cqpuupfx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ekjnsziv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vcmfsssn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ldqtskdw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3bcjxxaha.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qorsvjff.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3axmklluf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3bwsslqnq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ndcswlyr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3unwrhxva.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3jipujxid.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3btcfpzfm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xehirtwz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3fnifwojq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3tiknflde.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3rmisploa.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3lcfyhvyv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fglwfrxo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3reyfvbcv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3negsozyv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3fkjuqjnw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hpmnyoko.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fhljtigd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3snlaszbn.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kbxagnrw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mjjrlict.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3xevalsys.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3yycoelra.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nwoepijz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3fdyukfxs.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3royofrap.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3yuqanzxp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3zxgsvkap.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hjubiyzk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3lqmyhwpo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3sdgodqtb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3gdcljxgn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ovtybcwi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3tytpasgu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sjygbgbh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rbruegiu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3jmewosrj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cfhmfupc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3fwasikqk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3gparosqq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3qlueclsz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3cjgsdazm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3nguxolfj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3uyurtzfv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3mmadddvd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rphxifwf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3dfoydbjt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sozhriur.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3asuwdjse.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yhxbzldf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xyqqgykc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3sextmujl.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dcyhlkaf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zuzdvyhn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3iuknpibw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3svwyqujh.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3aphqjtxv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vakwkmgo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3sedtxnes.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3eeyehzaf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ipjulmfn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3xwksgvja.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3uruihuml.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ucxtrywb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3sofukhco.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzgidgfr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3lndvacto.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wafwpjbe.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3czjakxoz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3euryqmlt.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hbrnzuob.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hrfsoghl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vjobwhpi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3kwqmvexm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vhczlabz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3xedpevdx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3pkqannkk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3rvruhtgl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vlbcszan.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3broxvnhp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3qppvyroh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bgofzinw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3egbrvlct.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3omolohnv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3oqnjxshs.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3pyvgkvqg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3psyriwyp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ocmktpnf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dboixrmn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3oqwtdnmt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3kvvroiov.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3wrghtcah.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xyhatpok.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3candcqnw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uxxxmmzz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3kvisczks.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3yxxhrdbg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hsuwbwkw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nsurxvbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oocftnxz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mtkllgdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxbubqkf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ebixmwvj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hxfoyhaq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vaenusnq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ewofsxwi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3tigwykuy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tpettnet.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3qkvntbzc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3mnzcejop.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vpxoddhr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3luifoknf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zcygqrun.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zkazratc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bgikchng.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zmczucyq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3kcmkleqs.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3bhvwpioa.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3kxxruaea.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3xivoaofp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3puacsgnn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3izezlxlx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3hajartpj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3colqvfpa.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3obtjsime.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vcpxjivd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ttlqbrfv.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ktqulers.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3wbypczek.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3osqbjzop.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ggzjtnyc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3gkvsqdcw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3prnallxo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pzhkyenx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ehnflrfi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3isallmky.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xpefpbpw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3cfpcffud.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3lfaokgnq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3qzwkxxws.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3yjqjkcwl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3pellbtkx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gqbyimin.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3iccsrmjd.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3tajusddl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3sfteoied.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ughvzqoz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wqxgvcgi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ublmwsvb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3srfzuwqs.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hduavsqv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3yonwaoxw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3alxedjvd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hhhpxuai.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ewqthglu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ghmfavyb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iathqdet.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3fbbbhzzb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mjoczgnn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3xinuhjei.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3vstlvzyp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bvrmyfdm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dlyvstqn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jepoxetb.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pwplzuis.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ggpiikvj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hjlxkoyi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3dibsoltd.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3svqyvxwu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3bpqpxwxv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3dnakgozo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3kwzxzpse.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oyuveryr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3etrtdajd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vobxfslk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3rzmprdwn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3quehuhdj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3kskmvyxt.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3chqsdiyn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eaisqtjt.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3crqstsob.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3tfyrnicb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wilxpocd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3kaiotqdm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3sipvvlsn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bhljgefk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3guosnrgf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bqigktmf.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3eqfbywkx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3sroiynzt.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3zouawhhn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3onvptwbj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3natawebk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkzwbstt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3avgcgdnr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vejdsnmm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3qkfarwbs.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3iassfagv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uuifacot.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdoekwef.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ousyngms.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3czirmyoz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3yjkqnuwp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zhkowcgr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fpjpmdui.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rcbyhfla.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3vcithjpx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jxamztwo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xlxjaduu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3klszrxam.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bllpamxc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gnoxlodm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3xjezjbrp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tvqdeunl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wdnndzmx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3couuvuqq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3kpkgycuk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3pesqikhy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3vwywskjt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3nafhvnok.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3znvwxpjl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3rammbnab.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xfamtatb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlozvftv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kbocqyhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ioowdjhq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ymqbeity.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3hlwxfhmz.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3cvncflpu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rcyipfkt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dtykiljj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3urxlsems.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3uiffpcrr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3evjmoxvu.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3veudayls.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ythyyrpy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3xqgtodyi.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jschcchl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3xtqirsia.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3tdcnwegr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ogrciyvx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3nlxvphsk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ezgadqjy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3xthuolyl.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3iiwymbts.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3uxihzkgy.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yiydfznx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3cwtjsthy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ygbigwvz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3doeembhx.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3lcxtgigr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ocynxnup.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3okzfulbi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3vsyyajir.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ypcnwzxj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3xccjknzk.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3sogqbxky.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3wakwwcbf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3rbzlmrnc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3seoohyjg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3auvxklym.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yxlibhwf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3iwmppqxz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3jghvozmx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3xaucmlka.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3mruwjbga.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3dhnftpfu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ptoqiewn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3gopeydsu.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3zyzmvmgy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3qylhcwrx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ybngxhli.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3nencsjvv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kqwdsvns.html


<!-- 参考信息 -->