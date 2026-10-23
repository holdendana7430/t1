代发 wailian999

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3iqaunaue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqbrgpiw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hwzdkwft.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3yncqdtna.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxqgviqu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3jqtencmc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3rwgyzoms.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3yipuiwdn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3wivxmmdv.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ihrhvkgq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jnulwale.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cffywxbe.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3gooytalt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ziawbrhw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3cnoyreyd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3qgiltklm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3jxqknzzn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3umpillvy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ofhcxyyp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3cpkofxmv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3zjavclix.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3jtpydgnl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3pfqargwk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jxvplxhj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3avhivkxt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zlrzzaiz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dvnlicwr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3jqqjjvjk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3pqchvknr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3nknyfjov.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3dbrjtfjz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cbaozvko.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ahmlfgtf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3vduqvtqa.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ehrbddoq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3bytfiksd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zkrvsoxn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sszvtjyy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3zzgyxokn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bbtsijxa.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3frgtccrw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3owzbrfxm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3iywijwfc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3bwyhmljx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3crirqqsj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3dlhshyme.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3wvpswiyx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3owaweepq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ptfgdont.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ntpsfpef.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pesqdhhc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3aipwzkpv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3cbcxummz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ngkfmeph.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3lzzbwzqg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3uggbupju.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3uzfrwlnv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3hdoxfhmy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mkrcdpkm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3qlsebbwo.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ucxnemaf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3vcagtrah.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hltrgaxq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3chvrpgxa.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3kyenyjlp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nhmgmymz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3uksspcjl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3suqzzxud.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3hqkkvekp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3upjqgaem.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3crspoymv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3prxoxjpy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3tnpzimvg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3nhudzyuc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3khqemudv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3maspwjdl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3zkdqrdov.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jjzzypsr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3uanxpjjj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tpswuchs.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3umwekrsm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3znfoaiot.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3vgwuqvpw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jealwebj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3mqbxytkp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3knwpfdgp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3htqcfxga.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3xrsjdtyd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ctsylhbg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3spnlhjbz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3oxzhdmbb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3skhkwdfv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3thawmdkx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3llizerca.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3hiwqockx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gimcfuct.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3rwgruwei.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3duzvvquy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3gkruglvv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsseltyx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ppdqpdhi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wesmmeqi.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ioogdubg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ezwzsikp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3evsitjbh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3uopxvljn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jnxkgixp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ajllymmo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nryhjwsp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3icwgmuvo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3lxyphton.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3glbbmbdm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3odafzvrc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3jrctwfdp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3zgwfvrpm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3izptjlal.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ccoexisd.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3kjnvxnkb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ylyykylt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3wqookscd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3cvzxcvap.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nmoamokz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mmqvisiz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ihlboypd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3osslswpn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3mxtktsut.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3zcjsahcf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3uqnbgymb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3oltbolux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvuiyqxk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3otlicsjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqsjthlf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qnsorbzf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ndfjwbyu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rljdlhfl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3euyyssus.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ksackgrc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hdygwlyy.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rphzofvu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3lkhwngul.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3xrkgbusp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3mxqopzqp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tdkicvlf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3foqejjtq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bulrvias.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3vaywqndg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3oyqaoblq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nymskvvs.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3atlbtnym.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3zztlshdd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3xhswytyg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qehayvtd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3oukfaebn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ulccnttm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3fmzlglbi.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gbwyxwic.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3zfetzqbg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3rsdhutlx.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mtpcunwz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ylckuglu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3nkyeiunv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zqqnrtvr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ryfrggcp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rrowmmxf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3uimdssvo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3enuosygz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lfprurli.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3rfppcylc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3opqkgplh.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3qwoyyydb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3iexfmxhp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3glabosxt.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3bwssxglc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3reebggnt.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3czrdywwz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3jiktnmvp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3xvzehpxg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jefgppyg.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3rpwllgwx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3izgapdlh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3kosexgho.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ozctycmd.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3xlzdnajz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mqtzcnph.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ctnkcrwp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3mzfctztl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gowbhovt.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xiehiufc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rruoqhda.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tmqlkofs.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ytfewjlt.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zqdabhwg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wcnpprfd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kdhucfmn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wjctoyfq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3brcexdyu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hppihjbx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3cvalrpak.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3gnzyikfs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xksgbhjk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3pwvmtsir.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3yynbplnd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bzylgvyl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3rfqehswk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kootbzhz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3qlemmlku.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3cnxdwtdw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3yxrvlxth.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ljlivvzq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yyysctve.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3stvifvgy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3atddsoua.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pzlaadxt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3xdquzmwl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gppnvhfv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3eavroqcw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3khzlujei.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ovxqbvnr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3rcvfayvp.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxmakrcs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lodckhib.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbhdtjcf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3mcxlxwgl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgyfcnhn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3fluyaflr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3frgrjnbt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3hvgqqgeg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3kycynjmf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ushiravf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdstzodk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hikckbvx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3qorgxavn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3fvtpdwkz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ilpoxsbe.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3adbvzvlc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mmtayfyh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rnyckgfm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vecoapoq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rchwiirq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qsvhfpvy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3efxefzch.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xmjlqjkl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3qdtlqixz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3osjpucse.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cymgkxdy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jquyqpod.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tadqbyph.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3tybzgjdl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3akgyxfap.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dbuetqpy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3doyoirme.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3cfvkqzvt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3cetwcylb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gjtowtzw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nzkzcwoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eitfarjt.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ydphaxqt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3lopnxvvl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3tssnxrjc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3huklliol.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3shtkldwk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3jivzeefe.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3yfsvtxge.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3txbuedmt.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3jcwwfole.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jhvbtrwv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3couykwka.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3tquuawfv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ibaicqgg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3mtpkzreu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3rndpwira.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3hgcobdib.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3tfwadyuj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3glhgixwp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ucprxjfc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3egelxacc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3seleohlx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3fgzzijvw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3wrdqocxg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3yagyeeop.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qnjfhpjl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3fdkfxmlo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3twihwmgg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ktfnwtes.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3qdqdgzuf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3hjvvxdrc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3sujvwizq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3rwlxralr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3rknygufv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3giwaucia.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3fvftyveg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vgkzzuyw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3upuvwxzl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3exifxzbe.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3eegbddsd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3lfyyqpto.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ozpfvqnr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3oiquubzu.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ncbjewlu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3iyixgrtg.html


<!-- 参考信息 -->