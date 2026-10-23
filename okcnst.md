代发 wailian999

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bktdldtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nayfqjfa.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dsgprnox.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3zjocxeca.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ybeetstf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jrztulea.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3eycjggsk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3hweawgaj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3qtagihdt.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3lrwbvwup.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3assxfvbn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qkflwvsy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pftauels.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pipfhfog.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3shetyqna.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3vmhnwgmd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3fitnphko.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jrklrszx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3xccgmwwu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3irvzopaq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3awqurlhu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3zhnkjgup.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ydglqhiq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3osmiqwbg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3mkkfqsdt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3owktjlca.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3khlhcpve.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3omcpsvzn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3efvyfjnt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3nacijkcw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3fgzlupgz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iwwdvkcb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3qrgipyqo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xzzwwfby.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3hmfslxlk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3xoqgziql.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3riqvonmu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3krkjctmg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3nphxfrsh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hvpagnmp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3bahyhkye.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3pnhjjpkb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jpziozmm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3nzrlwbgu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3aoulqjpm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3vfvfaqsg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3dzbtalcb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ctzliivu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3rugmalas.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3lozgirha.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3kyrnqdmf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3sqmlknji.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3lpxuovwy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3yyouhaxm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3mgabqsvd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3cknztyhq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3lyynjgsi.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3kkhfxtoe.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xpwlnarl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3hqkexkhz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3dnorukyj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ncidwfsy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3keaeyjjg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ptpfcwbx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3aythwagn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ptfudgbt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3azzjvlff.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dffvoryc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3xokydqnj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxcvvkpz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pisyokyg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rduvqcro.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3gvflpewj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3uckhmylg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3fakjfadc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3etkzaluf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3twyzwlgy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fzjyvegl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3hrojxmxz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zofzxwun.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3orxrmqwj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qltvcvxl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3hyrmbpug.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3plhhhwbv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3toebcsjo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3yluqbjor.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3uxeyvhql.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bhwrgtyp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vhndxuzf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3shwcssyn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3icdqsxgp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3fziznnly.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3obapdyzz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qzvdscin.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3uywcxkam.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3wafkqjyq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3gcmwlujo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3wccvrqmo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3yzdquufo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3amxepcld.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3fgykzedf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbtwthmi.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xeekdypr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3labfadud.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hlrjpmdz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3niopzwqg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3gspkvghu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3pndrdubd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mtlnoojt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3xxnfpdyj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3uoiskdvr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3kirvzjmn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3gzpchnwu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3atcgwutt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3boimyxcq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3teefzuxa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3czvgfckl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3jmntfxfq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zezepqgu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3lbxnabjs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjkphwvv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3krgwrjaw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cfiweeno.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3simuwtig.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ulwtejxx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3kkplrqjf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ikdigjea.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3betjqica.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3oisctooc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afcacirh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qvxsdkzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvdbtlfu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uxfeykym.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ekhycuhm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3xmxhoxcg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3grctyysf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3knhpyoty.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3efnumybu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3glxuakwg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3aqkzqenz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3apkexaba.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3clakpusn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3puklyliy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ivfbxsxl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qjtsmsyk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3sodvkyue.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wkhkauke.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ukddbidq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3dmassdka.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3aauquhwb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rmbfftvf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3rsnmdxya.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3hbpearee.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3fxqxorvp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zwpmqmql.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eogoabtu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3jxugvxqt.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3bvbzxgiy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mskxnalh.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gebicnhg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3elruvbxx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3lbbrwaed.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zszrmkbw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hvljnwlo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3oaegpycf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ognrmxyt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gghmkqzz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3yfoczuib.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3hofclodc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3pdsarkxu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ysxkikzj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dhkjdghs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3xqdpabdq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3pnywwhkh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3vxszhamt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zfzptoij.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3bkiozrvj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tdabrdqf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3zimuhyaz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lexgqtud.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gubnaewf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3jjsuunbg.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3sqbjuqex.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dyvlycws.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3fdakjrll.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3pwwlchan.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3tazfzbnf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3pvyykaqu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rrlmmbbl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3miqhkiuw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3woskwurm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3xtxpvuly.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uqysxzje.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cjlfrtpi.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3jjpsdjmt.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3edfucjdz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gidbmhtf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3gxkffqsr.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3dxptkhzj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3xqvatblp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3jiwjddpu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3exugwmsj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wmauqcvt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3dgevcqjr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jxnhxopc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rscokixf.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jwqjapja.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3dnidbjlt.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rkvbuomo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3dmqkffev.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3fnvlcado.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ymbgjqyl.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3enxypyti.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3blgrxkaa.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3qxuznmvf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3fbhehtbe.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3inmzzpql.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3irigruta.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3grmsxmtt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3yismuyth.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rijafeeg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjvlgrhv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3vyucvzxs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3atnuypwk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3hpziedwn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnzyspgp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3gvdfdnpx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3gmjvpbws.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3bkmdgarr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhqncudi.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oejeplyk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ycntzkxk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3lgvghziy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3byhakdvz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pyheczdc.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3qyotpqby.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3lqxizqbd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zddkderm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ngnuozjg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3eekvarfr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wjmbpkdu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vtqygiod.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3brxaskqa.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3rpsbvqgi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tolitiob.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3snfimeqd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dofnrqiu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zgzkskzn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3czoqbrjs.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3xlsuoikc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pvpyckrj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3pcpnlydf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3bhwyaxar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewcipnln.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zgcvlwzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbdqhoyc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3fckubioz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ylvpyewl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3oeefynsb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rpntogir.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3tgtqppat.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3yhofavok.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3dfqlldqu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3efyenynd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3djaywjzk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kgpjopxt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3bokamxqf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3rnpamawe.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3bdlsambl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3darabxue.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3kixnnllv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3oyhedqzs.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3udzpzztc.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3lljhglou.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3zobokzbm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3hmrblydt.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tsctimir.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3xmoyhlqg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3oogzsubu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3jhvffglm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3kewkmzaz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fbujwmay.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ifimjocm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mwpbdnlt.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3wuyktxaa.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3vyawamht.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3uyspcgdo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3gdzlvolk.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3voglztne.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3npjzffka.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3zdqilngr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3nhfgvmbm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3esuwumfv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3luexvqth.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3jjxjpwug.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ocunodib.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zjbnzyba.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3qpfvbnea.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3nfuiiacu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3nyfsshwo.html


<!-- 参考信息 -->