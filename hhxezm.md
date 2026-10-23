代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3vdcybbbm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3btpqtddi.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3uimxuath.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmnsnojf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xjmajmhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3syykeavo.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oiewgrbf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ztzucmtb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3zqsrycfy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rkvobyvm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3zscpzlaw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3jngkhdaf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3gseyyhao.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3hsdtqqxz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3xquforng.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lhhcqfor.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3kagkxkbt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tstxqymd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3bijawzgu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ogykgyzm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3gfcbnoam.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jevtazjm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3zylluvgy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3gwidsmon.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wkfdardf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3pfsesmxb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zrgigyka.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pbqxvsbx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ydpzdxfv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3kzaeffiv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gvusocho.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3yrioccon.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ncccekqc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3xemshdfu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3vjxakcsb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dzeutcdx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ljgipqxv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3oxxxcnja.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3tnrjnelu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3chwthwsg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3swvzozsm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tmmzcqev.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ndgbhizf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3yakqplrz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3jcoupjvl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3dyzgtrhq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3czeomygt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ifuumvna.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cofcyvjx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ocdvlyca.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3fanifpub.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3uixunkhv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3gngxxfow.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3jscnouyq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3digljoao.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kwkecolk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3epohleoo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iduvngiz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3hutobqxl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3fezftotx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3jqeixkne.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3eeqwjtys.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ehrroqid.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3apdsbzsq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fntcynuc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3tkowftmg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3rtetvnpd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3rfmubvim.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3frquwrdm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3dhpqyvbg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3iqwdpdyg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gfohlvbd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3oielmkpm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3kebblgux.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xtmsoklw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3pbspvoqi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3iagjebti.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rtltfhmp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3wvjfyqhv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihzjrpom.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3fkgtlzke.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ghmmizft.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3zpqhjkdk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kkbtwfbx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3blixtwch.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3cweatzxz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3erkaaixe.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3codcelod.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3hsnygdqo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3kcjnpvcv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3yzsgghyd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yyyymktt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xnsnczdb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3jlgyvmxn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3rifkunvz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3miqxfmiu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3pjlcegxy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3cpogbxcv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xtjzunii.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwqunxnu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mcpmrthv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3odchrwac.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3lyiwucyt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsebhzkp.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mvlrorrn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zancbfsr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tieyxmgk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3crzlotsh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3lmflfwip.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3dwbyttnq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3edxtdojb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3iarjdcks.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rgodieui.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3fktvarmo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3yuowvfkp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ytvfmacv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ukjflltn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3bopjwwkt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3txikadzk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3degwlfhr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zowdvita.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ykipodwo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wffnbtoq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3sklxtsnr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbwvkxsy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ypqvnaea.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3gprqqyts.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3erzkjpqg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jebggipf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ccdczbgn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3jydekiqa.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3gwlpszjg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dirbrgxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brmihnum.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nrypxexa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egfvyqsf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iiglunxo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3idswpggc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wzjyajja.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3leivvimf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3zwzoemfa.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mdorrhho.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3dhqdgaju.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3xlenovgk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3girlvrhq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3aajwkwrt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zppucoen.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ubqtzaaz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3urrqtipz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3csjovyjk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3lijifcfu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vvqmwiir.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3qtnlpgmt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3jkztzgtp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3vltrlgid.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ebytgxyq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3fxfjjrak.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3dyszwyfl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3foaigtus.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rtglkdxp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cjdkbagg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bsgtxnya.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pzupqavz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rzdckxvo.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3gxidmrqj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qardzjtv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lihudqqh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3msnjlsnn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3cdcryvwl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3trnqjciy.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3krxvjgbe.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3eoypczoe.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3kkspczdf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3gfbqqnse.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3cjmzernj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3snvflysj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cxsoulxj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zodjclpu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3sqajcgsn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3mvfdssyf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3tfgftecl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yqtsvtoq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3jdncpcxe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bvlqltzb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3eamlxmob.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3nohpkbil.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ucdsruva.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3uxgcaqpc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3imjphrhz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ortlitbn.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bjljzprh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jeezqxrx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3gjzgdwgj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nqkapyfu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3gkaqoszm.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gzjypkgs.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zkussuzs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3remjdqwi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ebshtqpi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3uvzecxkv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3zoighmff.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3hkgrgkwu.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3leujeuux.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3uumcuncc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ugxyuwow.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3kjhhhssr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ealgtyie.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3adojoezv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3krghgonr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3lwuljviw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3klqykiwc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ouykmhnc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3omxtygle.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dliobuar.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3vfhpxwwg.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3tbnehxjn.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yoyszjff.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3hbubssvm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ygmufovx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ggeusnxa.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pmsezwmz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3aljigrcj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hmpmbcdb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnmmxszg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3tesuihug.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3noobfzvg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3giittetq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvmupgkk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ddsjttnq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tccnrlmk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3drsighsu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3esrpulry.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3aufpfeqp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mczlbdtm.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yevziyhi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3yovcxrsw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3uenkbawr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jvkncbcm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tqrjxjli.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3exlupurh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3tszhbpvd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gkudpuhe.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3pixgziua.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ekpeyzzo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3yepmnzey.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3edglyuxo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ackuwtmh.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3jcbirpdx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3oihapriv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3flrvtxpp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gcafejzf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3dfpivzpl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3npprpnqd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3mxznewda.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gloylsnd.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3tsqnfqzs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ghcqefpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tofyoxzb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fdmlaorg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mfhnynkg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3snnhagjm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3skqqwimi.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3kgbofzmi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3orstmyqa.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xevwtgpo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3yvhpubsj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3qgmuvtby.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3hxdtuilk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3scxlfjnv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gvyyanyy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3bcxbnmir.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3zkxiibbd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3nhuvwque.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3shamtkem.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3wwrayyoq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3wrmvpnnh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3teqqurmh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3qanmbjvi.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3elplwlkp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3svaintyf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tnwtfsex.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3xeytvhli.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3axgyfmfg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3yryfbdjm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3oxeqgzsb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3uialzuqz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3nlitqbcx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3pdcztall.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3vztmmxvx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3fvbwgsak.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3kjszosfh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3jrenkfgk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ueztmsif.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3bnvblizi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3isewjpih.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jsuabscg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xstpkasx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3cmddjlbx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3tklukojb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3hhweixrr.html


<!-- 参考信息 -->