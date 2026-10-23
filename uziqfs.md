代发 wailian999

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yyebvbmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jaznlxzn.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bpgpbcvl.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ztdyuirb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3plvjodkd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3sfieznyx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ssqjiqvh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3uuubtzdm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3gvyhiwtg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3exevoymb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3guyattzp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3quzuiooq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3mqmxipgc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dnvfthmv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ahqochip.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3eqrxpity.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3uekyxekc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3umxgxpsj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3dslevycl.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3udhzfila.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3jrxwozuw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3rmwqxrbv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3jnumypug.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ialcdlyk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ynpwzlcz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ocazwyyw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fwwynboc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vgcmizfp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ptfkagqv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3dipwdaxs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3xzqebsig.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fzgzhgjs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3vuodbyxh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ndirxfha.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3lwsgstuv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3pmapnggx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3imzlgfeu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zhdlgjhd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jizamkqi.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3eduwjbcc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3vkvegdry.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3wfangyws.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nchafzme.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3jksvjsop.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ovvrqqsi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3oexvasts.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3bsphghon.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vopvwnds.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qowlongr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zxnhnmlv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3rfvcybvx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ziplegai.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3fpgbtmgh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3rrvwyagd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3dopokfas.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3mumanlrt.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3bdunchzl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3sckjjmbt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jmrvsbiw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3lugpzyzl.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3onzoygky.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3cjeewmuo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3qblrmcot.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3gnopfrtt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3dorwclux.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ppgojvql.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ssspcmei.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qalughfq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ausqvxkb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3glrrhubi.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3fgidsjjf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hmblstar.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3jfkryovg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hknhwttw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3wqqfscwx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3odvlgksy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ixomgxuw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wppebpdl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3gzrfxsvs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rendfxpj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3louworxm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3zhfdcagr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dwwaxquo.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wlokxbgf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3luwcogkw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ymidntxh.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3nkprjxnz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uxxwbnvb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dbsdlejo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3lfqifqxp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3yvpuzwau.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3bsjyvmlf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3hakwrboy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gqdelvix.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rmdvewuu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3aihdxtbj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ikktlego.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3algtjowy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3cuhuboeh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrobjnxd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3irefqyxy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3esbnbtfm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qjuhgppb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3altkmxsq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3fcpmjmdo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3zmikghfq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3yllggsyn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3thecwzdg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rlphedfi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3rjskwyjk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ypthqtya.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jjqkokdg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jtupsdhy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3obywyovb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3amknwpjc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3feuhgkaz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3haofkbdp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3tgyjnwpx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bzilmgxk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3zygyfapy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3cncllmry.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3zgjzkjip.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3lnwqoeff.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nhxmtuyy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3hawjaizx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3mhkmfyxn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3qsmsnadu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qnnithtt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3asafjhuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ssausdse.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mtfhuamn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihiefbnl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ocfbfbao.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cjxqxswx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zushasaw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3jyjxlfyj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3zeviwlxd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3cvhrqcdg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3oabunwyl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3mknzlqcb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3fkdnsuwn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3zrdncmbz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3irjpiybl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3czyqmoqg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lilrchel.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3pddzixtg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3gixckuyx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jeojrter.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ktzhjirg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3cbctnkth.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3jlelcfjv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bfzwnskl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3twjlxrfr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3zcwndayj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3xaosfxhd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bvojhgyw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3dwzwiklp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3umnbsypz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3sqhtspfw.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cvqxwfpv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3edccjsuq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3dbftrbrl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qtcgjjea.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cntxevwz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3khlnficr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3iwlkonik.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dmwnmpvi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3hlckwhen.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3hmogrohg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3imfrhryp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3vektagdh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ycnkqgen.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3xfyzhatq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ylljiqcy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3gbmbzxmy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3aaquvwan.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uycdrvcl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3cjuqewca.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3leaqmyiw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ajkjiepe.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3knyskwqp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3eiyphksw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3vvhlqrzs.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xvitovbd.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mjclslpv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3bdhqvtwy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bzgoireu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3vzhjeomh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3esmyqgpm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3qfkplghf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3skrmcfio.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wencjqdm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iindhdqq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vyesnlha.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wwkvtfyn.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3krtmgrlt.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3xdtdqhag.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3suhmntso.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wcvwyoec.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3guweunnq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3nyoeuvlt.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hzqtjjgw.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmdiiusc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3nhgafcuz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3cmqcijws.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3oahxgudm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3euidzgfj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3wdkijqax.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wyjbiuzt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vopdpifi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3jpoldfpr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3mxjjpofl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oqrgzsje.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3rceismkh.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zttepsph.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3uwoobush.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zhdxuiow.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3nmtejkgs.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ajlucywg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3diijetsg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nitqpohy.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3vnpgihzw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3bpjafrhc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3quxevknx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3gckafffz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3camrpjiu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vhkwodxo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3rvpftcio.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ntmipjlz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3goyqects.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wphyxqwo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3oborqkmk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3jgvwtlsr.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3faavztcg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ziasxdzt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pmyfuppp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3fgvjpcdn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dpmmifob.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vhcaqpia.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gzswmblz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3bpatgiov.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bxzydbef.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3wvdednxg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ccrqvghm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gexaqkso.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ruraroym.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3aejvmzuc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3blvnptih.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oahsfsiw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3eftlhgzw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ixdxpjmn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ajxwypbk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3skjnpyju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmgjcgaz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mbzhouut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jljunnoj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3evpboiwn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3eypadvvw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3piperpuc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3muysfsju.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3tanigviz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3bauwwmws.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3piiyzkxt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3zxshcanq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3sqraffzp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mmrqmznv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3lgjewokw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ydhgzhnn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3fllbanil.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3whuedipc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3vhcpwxco.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3etkqotmg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3jpicxdiv.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3mkzkxuap.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3hccproif.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3wxlxfhyh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ifdglgca.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bwtlfobl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3vvjjmtwj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qiaowqeb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3nyxzkvtq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3bpvaglfy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3htjzfamc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3lwexxcsj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3lloxmzrn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3cnbhspam.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3oxjwvpfk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3bjodhdin.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3txdrqppw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3cqiuczjd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3lixcpcfa.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hepkejjr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3qrupgufq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3pjcqinrn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ptnoazmy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3kicxukgl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3hsppfjtg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3wpswtnjv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3vytanudp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3exbwdsmm.html


<!-- 参考信息 -->