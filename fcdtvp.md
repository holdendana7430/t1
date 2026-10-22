代发 wailian999

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2jrjryjee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubhsyecf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2toroiikb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2hqtqiqzb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2knfkdmye.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2xealogmo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2dhjaufyf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2sskmrtsd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qpbmzupj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2zjwauvoj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2lahzjike.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ycednqkq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2btppolrd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nmagpwhw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2flkvlmpy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2tyxcnudv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2rmfcmlbh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2eyxujlml.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2wxsdegjq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2hexrcssz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2dlesvuuc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2blsifkeu.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2eztkqewv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ymjoacvn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2eswnbppg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ztlpskgc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vqnajsrl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ddawslnp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nhtghqfl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2powuenqt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2srnficmx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2bszotpsj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2okipelkp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tabxyfvp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2njdwpmmc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dvotyauj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ukrasxsp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vioqyqyn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ksqdjqwt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2civvopkh.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xsnzjdkq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2geuedxid.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vzbdkuml.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2xebpyyld.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ivhxxqxl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2wjeprzbx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2exxxptmk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gfmdgoaq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2gtqbbkbm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2wdrlqqqd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wegqyved.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2griwavid.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2cbtvzqyf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2nrseudiu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2wilptmjt.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2pqzpvxxv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ehwrlyfa.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2fafjhlku.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qaikzjgl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2tkgnetce.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kmtwooqu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2gexcligy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2hsfqtgrb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2jofxzoxr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2pwmwoknp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zyxhrgou.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2txdacofh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lqgpoglx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2cveinewo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2whqnevnk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xztujfum.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2dlyrjznv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2tkhfottg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tfdtpgtf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ybblmzaf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2wphubqbd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2quwkmuun.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ewyervap.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2drfoxkco.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lrvqjmaa.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ucjqsgdi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qfpaahmn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2sqkonorz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tcylltqf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2kfhcfuvr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2pubgyzui.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2cutlpryw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2myesbvbr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2dpvmwdbb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ikewxrxf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2vacbwtrs.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2fjdrtsxi.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2pikmaiil.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2xvidyrex.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2uwhzjlva.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2mpsabeyq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vwovnnhf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2qxrtnlar.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ekmxyxxx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zzybrdjy.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2nnzjdqkb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2kddzbavu.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bazkryvl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2epohjbtr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hpiwhdee.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2phqzuyvx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2klydwvml.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2rnflfabm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sluvrnra.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2egotjjjx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2gsqbuqwp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ihydqphu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2dsppdlej.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2oeucelcs.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2rbqwjoak.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2vnhgqvuy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2cpsjceuv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2fsvxtpef.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gpvgaexr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ajumkabk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhinlhki.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jbxymibw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wofibhbz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hmochgnr.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uwbseovj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2kiqkaypk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vdvczduo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2rzbxfiqt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cgpgplgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqoupstq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ymdjkeup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exqflwme.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nfbmjyaq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vgbjupwz.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2afrhujlz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2xizdceuc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2dfytihyn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kewhioom.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2rcodkiwk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ymrtoslu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2sfopaxgg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2xxlfnrzd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vxoiukia.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vajvusdr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dltaxkxr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2hxlummhb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lvfvihyh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gamwojfd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ftdhnbhe.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2djnhrojt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ucfioeem.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2dxgzlaoz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2vpfntsgd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ppqjwmqx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ffghorsn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qjfyzqhh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pzeimaet.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2betbqssj.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ykbqxeki.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gthfbwrb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2manvybww.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2zcbtaycq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tqqcdleb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ifxlucnu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2zoplrsfy.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2mnvaipwj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ooobwumg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2aqhsdefh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yusjpblm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2hjllhmhr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pstgekuq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bjwvdewj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ezxuraql.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2jfsowunb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mwyneluy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2bfsxsvip.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2iozqkeja.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2cghioevg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2gnjecthy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2spokuvjg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2iebneivb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2pprgjjpu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2aajpzfjl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ipisvoxa.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vkhuskho.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2noylzkvm.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2wuvjzxaa.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2tfsbfbfl.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2pfynqvec.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2defrlzkd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2jyncamfg.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ynwiibis.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2toyohvdv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ewjttqiu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xekfsvoa.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2dmtttzea.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2pjvekvms.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2nyhwxbgi.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2tlqvfxcz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2vijobyla.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2zachybwm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2hebwjjgg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2zbgxfppd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2wvodilob.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mxewhsgl.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2vjcfediy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mbowllos.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2zbvahyqr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ocxxzkge.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dvmvwbby.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2gkxnsbux.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2lrncwwfm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nmojufec.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2fakvtvhx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2yyjqxczo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2oflzabym.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gufjzmnk.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2qiucuctl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qmodlqfn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2evoacgln.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2afbgpfcg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkimyiiv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2stbekvvb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiocqzgi.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ztvyvgbo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nifnkoxn.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2bvwfqzsd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2pbwtqqfk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2drgdfbqq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hohrgonz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2htwkcihm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2rivjmmzf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ftfmcwtw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2klfktmpd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hzxjhzhu.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2tbtgegby.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2irfpweqh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bxfliryo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jttnvnbj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2btjrnezh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2huloqfed.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2avrexthk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2xyflgyuu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2eugibnmv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bnlhpcjz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qscpdamr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qxoscxaw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2bdusbzrq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2prnbfxqc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zjraehsd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2sqxhgeuv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ycuqxzcn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2yzmtrqte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wffxzqvf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xoinrxms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vsskfqpm.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2lwokyscp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2uhwgshqf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2aqomkzed.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2oefwmdef.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2almectgk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2mgrqmvdk.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2trxrznej.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2tuyvyyjb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2flbiukuz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zrffardi.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2acmwvzqf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ijlilhns.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2imadehbr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2olhvbwiu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2zuocsznx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2zhfgword.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xdwevirp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2zuaogwzm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2nuunttbi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2mosyalwr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wxxgbmpu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2fardvpjy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2odbylzhn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2guvitaeh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2popsrrfw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ptwfdwne.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2joulrato.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2zvfjwmgs.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2edozzass.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2nldpyopy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2xxrviwrk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ycvmhwpn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2oqbhviud.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2xovsadhq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2lkwqsaij.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2miiutvlb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2hqmereqz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxjqbymx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2nhvvdrbb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2dyclpasc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2gyehcbfa.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2gymlxmfy.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2yaaeddnn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ztexqbhb.html


<!-- 参考信息 -->