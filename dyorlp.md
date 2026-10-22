代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwltsuqm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2czwmqgll.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ycnyeoje.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rijmzivb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hreczdyn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2qegbdtmj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ktiyytjf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hreyvtqd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rninsllk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iqcghzvo.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2toelzczn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2stgvxyrm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2xkyipxow.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2kcylzmim.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2tkxeacqt.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2cvabdkeb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2bkeldpns.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2obijwiwh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ioqdnaox.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tetdesao.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2kmzitoyi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mlmqwxdq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jvijdecb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gsdhdxxx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2aagkefck.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2nvjhjgyh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2piaagkiw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rphzttlr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2gewnpthj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wzzlvtvh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2uixucjyy.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2yamyuesj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qckdoesy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dxlpvwnw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2dgwlccas.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2djubejka.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2phkdzugf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jqcxaaop.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2feelenow.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2sfymaeny.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2khwlekhj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2qcugotki.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2wasqbqbk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2pjprphxc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2pghcejez.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2aupuzztc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kfugztta.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2rsndmjeb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2xqcmtobk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ufnrojqo.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2rtjeikhx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2wqremldp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2mzxgqpbq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2akigpikc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jmusdjpn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2rxkqaypu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2udrdktzz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2gksgmhgl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2evhbkxpr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2utqdzzem.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2roldsfpl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jngqqthc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2qpemgksk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qckupdlg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2xwofowhj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2cjtsednw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ckhruopb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2sfstosbn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2voueixqe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gyvuabsl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ujhyaffg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2svzpgkaj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2rbxstguf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tzqdnpsv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2nzmgmkut.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ydhyqdsl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2jirzcoub.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nstoproq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2sdlysbhm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2agyuwbga.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2hppotgab.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2nemoyeck.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ekibnjyg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2guezqemu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2zfxzwumc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2peamrryn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2qdigkfkg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2uyjlbypr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2sgkingsq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pzxjkggi.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2mpdsqmhw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2jxkuivyw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2htqszbqi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2uyzmyeoi.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2cvopwxtp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2didxrxdt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ujkcftwo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2rverrvwc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2alyhydgw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2gcpfhrav.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2kfzfinxv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2lllgroge.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ifhwelaf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2amtkqnit.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oyrstlly.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2sjzwtopo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2xbrbfrzn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2vkmdojmq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2kdrtxrvq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2allfjtbl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2pllgvyqo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2pbmrsezj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2uibyhqfd.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bhvwrxcb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2pdcsdejy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2mowsbwyg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2qonxcxsm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2tsdgnlna.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zwzkajzt.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mwvkldyz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yfzetzum.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2dkveqbjj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2mcatcqux.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xyyydibu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ftvnwjnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkrmyxhg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2agnahjyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgghhemd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2txyjhali.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2frqpmawa.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2qbkyphja.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mopidgmr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wbogegrr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2stndxjyy.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2rfpovbaq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2cfkajynb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mzgsruai.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2xetyxwyp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2admbraei.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jibpckfy.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2yqbiluzi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2jsyorgwx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2pkxfjewo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dwcypafn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2bxtlwhek.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2elgnglxg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vdgzfcdn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2negspwdu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2sfbhemxl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2vlrdrqxx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2uoyfqgub.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hyezxnpm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2grbqwyui.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfvryacf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2npcibwdj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qxuhmwsj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2leaislbc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dtsjgyfb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2umzdvltj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ajabybqp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2apodqtme.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qfqqlfwg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ixfffzfs.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2tzjjlbov.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xeyhcrgy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2fewglkgg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2sauxmkjh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ilvxowcu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hyqtzjpy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2rabntnum.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2jsfzmweh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xscpvqfi.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2hljaxbzm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2txlnsxbw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2cguppvyj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2amzdhywa.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2vohxsuuk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2wdnnhmjo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2gsskzuhk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2vksswvlu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2eaqjjyjl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2whpkqrqz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2mlgqkzdl.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ioxhjxtp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nxmxjbyy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mnxolpks.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2iirghkul.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dypwxrye.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jgkgswhj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zotxktru.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2upamzvja.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dvancisg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ftgnvxqf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wtdcffij.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2aooucojs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2rhgxbgyu.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2prtonzpu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pzfxdmfh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jqlhuzqi.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ecjcndqa.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fujkjbgn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pksothct.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ogptecsw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2mshztwtr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gpfqerlm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wyvwgrio.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2dvnwrzqk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2yfwpeqqd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2subbzhkt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2rsmztcoc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2eicjuamg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2jysmpcfn.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gmtzvddv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2vbulepig.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2tttlkozx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2qixnlmio.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lvjcqdts.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2teqenkye.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ibfwiowp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ynglybqo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2fcrxuumn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2joziqghj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2wpfntnue.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2dezseckg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2fmsvrniw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qhwzfqkv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bixhokij.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2jkbsifzb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2szainxbm.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dtwljquc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2aoftwkjg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lzgwoldk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2melelehf.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vajyylae.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zmgsided.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mfvbzjyv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2qfcsuarv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ysxlpgbb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ronrjehx.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2nbjtwkix.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tgrvyuci.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2llubsmvk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2krsudxmm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2jebnljju.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2oxmjwqgu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xhchawqp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fchabwlx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2hmqjwhoj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2hwoffhso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2poirewff.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xrvvuykc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uscymviu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2yhcqtdhz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2xdnpjakv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xkfulknh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2jrhkqeer.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yjgkqkjq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qvylyacn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2wtsuhymg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2tnnmcirz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2jdlcqrhl.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gsygmkci.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2rcsirafz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ghcuruoh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ecjpcknh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2zydjgmih.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2zemcwosm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2fdsmmgsi.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2znokfytf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2bvjpmeaw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2asrzpivd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2khvwnwnx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2edrgsxtq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rbqztagj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ttpzzbqa.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2urirqqqr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2chievrfb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ijnnzpmo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2lrinftan.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2tcwrfgej.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2apqmxuwb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2rkwhepam.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2msesnjud.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ngilsoix.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2pfmaeafm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2rmtrhflu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ksrnjeck.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2npltmywo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2pephtlar.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2xamhqopq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2yqnmmlcw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2rqwpqjnx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2kqtqzjaz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2wppaahzh.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2jgdkpnrm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ebusjuaw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2maieywbq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2tzrjyyqr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2aclvyseo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ogjbafxw.html


<!-- 参考信息 -->