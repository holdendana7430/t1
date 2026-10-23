代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3suddknbg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3anopiczn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3mmfnpfik.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wdbricpe.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3xxahmkmb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3xmlccxjj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3czgimsxx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sygpkocm.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ytjxjaob.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sfjnuils.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3fhlqqkvd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3khsypurs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ybatwcqr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3pykpigtv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3waaqvcoc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3qdetdjhd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3riaobloj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3qcskewbg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3brfnpxpo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yulxqicv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3gmuqubtn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3bpexyvfq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ysztnyrq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dskcgpnp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3crozzjvy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3bvmlgkze.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ftpefrvi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qpdwucky.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3wqjhpmfd.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3qgxuskyw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3jjrinxty.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3zonrkgfi.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ctlrcjic.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lkswmtkf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3hsntdvyk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ttpirife.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3dnvjxtfp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3trsfwixk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uaxjfhnz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ykabbkkr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pfnvswup.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3sqqnyvjz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xyarmbok.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3zpiaeyfe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3rumklmgz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fihhbzpj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wiseipgw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3fsjprhns.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wporaath.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jgbkglnc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3bcdivicj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3hsausblj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3symgkxwx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3qvphdxgi.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qkzbqrkr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zonutdeh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3tpzggzkx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3nnnbjice.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3gjlqtlqo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3pdxvvsik.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rcwyobtx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3daqvhazm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3vdhuvgzw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gdxmbemx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3mtkqzihx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfamztsf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rzidosdb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3dghcfbkh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3dwbsiwre.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zxkhmiya.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3racnafvc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wajitoqd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3nlvkvrcb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sqnrhomr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3rtmczzmb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ryfwvtev.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ywlrmwny.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rwviugrk.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3iwdfhoqt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3uwssvarj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3brpdqzqz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3algykifo.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3katwkpqe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3jfkoympy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xvhrzmuy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3idjujgtf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3pzkvndnh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3rjlsudgm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bqiljttn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3onrntrqz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rrzausmo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pznbadrj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ekpobzoh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wjyxbhdj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3sjwssubd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3yowhyzer.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3klcptpnl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnljzaoa.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3klwcpmat.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qywvjdud.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3lgovpjng.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3yiulfaqc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3txvdjgrd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3bbsxyqhh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3oihmqlmr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3oacwpqgq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ouobalke.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3widzxtju.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3pbshniqf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3nczlalmt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3hjfderly.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3qeaqmhgq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gfflbife.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ogletdhb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ytvztbuz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3oxaktedz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3njzrpkfs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3oweefdtr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3alnhhxub.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vqwlckro.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wtzjrwua.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3gokjohxq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3jtqgfefc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vpbxvzkn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gdrdykej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pchogrbs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xpubrnht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aayckujx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nhdifiey.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3etgcpkqc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cpqvrjmg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3cjzummxd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3bbafvdbj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zhyhobzs.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3kdyablun.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3nhrfowzk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3jzzdlpgc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3qvwtthrn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xfdojvow.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vwznwzff.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xxrmkfit.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dvoafmwk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xoghqcgh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mgesrnhd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3usotlfkl.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3oudrdwwn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3nilqhpyz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3awilekiw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3jfqhxuao.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3wmfepomv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3uhaxqbkx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3opuzhxwc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fecycxzy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3mellzjoy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zfxpmxlo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kceeucin.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3fgqpwvcd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jwgcpyrl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3atqcvawq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3unxdifxd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3rislgkch.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tcisdrcy.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3crzhxprw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3nabifllp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3axgztxxu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3trjbxezr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3bvmcjmdr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3uwabwizo.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xkvigqtl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3bwzxadvy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3tckvexpj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3wvniypar.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oqutzhld.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kscotohy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3idussriw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uoegjorn.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3fmuydxgp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3wzwrkfxu.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3rdgpkpco.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xdnirfbf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3fntvgmpw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3sbwhhprj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3krfclhkc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3jbbttiwv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3idaafesl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3sjuijmwe.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3jbqevqfv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3suviadgx.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3btjadnhz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yorquvlk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ebgpdckh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nttmietr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hkncyelz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lqpvtvrw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3girrlkmh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3cvrruwte.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3xsviafdt.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3bsmohnix.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3evrbqtml.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xvxbgvel.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3msbcjypb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3tpouiuwb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3hlernmka.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jwqdkqhi.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ormhywjf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nvlctsgw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3rudwawug.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3vypmbzdg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kzffvijt.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ncjyhcjh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3fmpbumaf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3isblcbjv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3glfamlcc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3jqhcbdol.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3udzwcuyk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3wcjnqklm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3yrkfgoas.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vflzinpb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3gjkupdfb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3pcyokdrm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3wpstjovp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mympslce.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3lfygsoaa.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3fjazxfit.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3eqdbeevq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ancbcsgd.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fbvfesmv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3mxgtleen.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqoaxhei.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ojnmvayb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dlrzuaoh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jmgocoyf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ukdhruzo.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qfwgihan.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tusmeagr.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ymkwwdlc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3mhalmfjk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3azhkpabb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3xodrywio.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ienyqfax.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vcflvmtl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3djasgiuo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vmrvdmbv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zpsjkxrt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3cffqtxgi.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3cejpuomj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pgrjwvlp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3zqsgssnk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3wsdtzlrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sinfcysl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cyxbgeml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fomsohyb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3bkaiohzb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3qztfojgs.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3iookvbsp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3abkkcugs.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ejztzgea.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3oukuofnn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3upiurlql.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3jmbelgsp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3buwhnkzo.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3davsohua.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3jexswcli.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3gaholcfz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ywcfdclq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3vkgzibcr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3sqdudgyb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3nfkwzlfy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3bfuivupx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3vifuiwaq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3fsimurft.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ktjpamoi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gvbdonmg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3glkxmtgy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3opqdmzyn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3napktsmo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3pojtitqi.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3rznbalrh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3zllnyhpb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ndmrheil.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3pjhvxajt.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3zumcplfa.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3qphxwnjx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3rdacinlc.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3chdjetdl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ppmpruur.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vbjghpoy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3msrbupfh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3uecpaaha.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ioqwfhsg.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3qoyhqzvv.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ctaawuwy.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3etpnngcm.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3omlvrssy.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3btzmhhdq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ubtcjmbg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3tpfvcycs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3juwtshjl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3nfvrfwsv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3deukcjfi.html


<!-- 参考信息 -->