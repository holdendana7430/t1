代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3uskuheia.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3isxlzdiz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3xpjamihm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rutqjvnl.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3zxhgrsje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktbmaula.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fldobeil.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3bdddrmhe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3qcphsdqw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3uvgypxqa.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3gyfyubeb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3qakyrmxl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3khhonbgw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3xnddfyaz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3gykirlrc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gpsbervo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nyjxpfyz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wmtouvcw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3hlngpvvv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3vjhqpzxl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3rvubdufz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qhzsgcnr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3fpubfcmo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3nhxxmtvj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3obnyfkih.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3xzqvmowg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3cwoeivut.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bgithcdy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3udhsvwux.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ljwqugvs.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gpvsmwan.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qorbttqs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3eqpbebho.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hhsceqfg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3zerviixv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3kgnpnnub.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3hbqwjucl.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cnprpquo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fzsreovs.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ovsphxml.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3uqbehdbm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xwuafewn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3adqlstce.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qaisyjff.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3qzkxpnyb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3hsypdxbj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jesactsv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3zzplmflv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gpwihyhc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3zmpqdhei.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3sqyqptrr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ysblbqvz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3bpguacsc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3osdshniu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ipqkupcb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3osmrwwtw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3nlnjiykl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jfdwasyp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ulqgddcl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3lfopxmby.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3wbvkwbac.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3pemqbgrx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sriqkvaf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3sjletfje.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3vwvfbwtj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ftklyfyu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3acsdmcry.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3fbzhvdcx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nvefrikp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3enqkewdy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3jrhmdaca.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hidhxohb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3vimvjafn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3fnvxioyn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jsysnuut.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vdyylcsh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3jzfhkmfp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3djepegss.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3puyzeieu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3kvwjiyyz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3bmxbajqi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ghjzrsdp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3lzfqsbyr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ixvelvzw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3uwubnpxu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3fqotbdpb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3qxhutvkn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yccvjjcb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3npuwwjxz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3fmhlnrsf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3xiufgoyd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3qvqulbwx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nndjiwik.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3blojmpwj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3rcgqtkuq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3svxkunps.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3efbgamst.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jmfscvbp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3bwbltybm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xourkxwt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pnophvgd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3quaxtrgf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3bddowsly.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgnzlowt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3rnrynxym.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzkyrfaq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lxvampov.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3dqlsmoki.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3tmhwrmxr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hztigoqk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nrjlpnmf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ielnbrwi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uczmtoxg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rnwcftxc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3havtqzqy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3gjkyhgyh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3opgnknqi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zkttqajp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ndhryeco.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3pmwzbwds.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3hosbagdv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ukvwmxhs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3htatmhme.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3zmthsdyf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tziqnmcb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3lyqfrffo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dttxmkwj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3zxmvselh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3igpsriye.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3arynrkwv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3iwtadjqk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ypkxdklp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3giymbyby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyskjqzo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3hadfxclu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nubraith.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ouuptjrc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3crmgoktl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xhxyorkz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3nmhnccom.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3igcrpbdh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wzbwfjzb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3adpslqww.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3psrqlymc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ycibqicq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ltnqvjzr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fkeokqbp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ouiialcd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qxhobbhn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3xrmxwghv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3lxddzqhu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3uudoccnq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3lwnapsbs.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ekeiuhkp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pewuzqzw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3rcwcvghi.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3gksxeqah.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3mgberzeh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3sgijxtin.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dgebtvah.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ipknonha.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3rgiohpys.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cmzzjfdz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3whavdgdt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zzivnovf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3dbmqonlp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aiqozmau.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3isvdpgqy.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ufwvsncv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3rokeuslf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vbjiobsv.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ongfvhvl.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3modtncen.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3loynlnme.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3epngkgty.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3vfsjlbqi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3cmcgdnmx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3tmgkjwlo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3abfpwznl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3unkmqqzk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ukeuboqs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3xvweuhtl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3skaqtwvw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jjqjazbw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3sazgyxza.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vdyjvvxt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3niuuopca.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3uwewtvwu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3fdbscfqm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3sqtbasxg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zlgjnliu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3bvzujmun.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3viqxjaqu.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3dtrkrhjc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3kprmvyvo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yrrddvei.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kpekhdiq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nxwadmsh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3pobhnvqc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rmijgocx.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tirwtbsu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lmjrjbdg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wltshjun.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ijuugmaw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3tonladpq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3skpmlffx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3gmyhbqan.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3vvuoofzp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jumgkvzw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3dzjtrsae.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3syvzkfne.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3nvuxajht.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rpyxfnyu.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3yegsgzwm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3gfzecfoj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3cqdewlxq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tymixzdu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3xjfdsutb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3umupeedn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pjwmanhs.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3stcoxmjt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3hiwbollk.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mxrfpack.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwjqqwhi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3dcxsbrfo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3edothnkm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3guuhaywx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3sdfcwzcj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3rufyycoo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3bpksdteb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3gayqyewi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ynpotchr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qndlxkyd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpctyknd.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3byklnvrv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3pirtnagr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3fzfgxnil.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ggfztbli.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xsvshkgd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3qkmedbzx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3mqsmdvln.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cxzfxogd.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bescqocz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zqjnnyzg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3autkhwzo.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3creeytik.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3rylnmtby.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3djjjlngg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xsoscoqe.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dyupchlh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rvhecojt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3rpdnrrwo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uyupfbpu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mjjtdzys.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3khqrryup.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ykfetjfj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xpvqnyma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tplroaga.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xsvwvnve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hsfaskrt.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3kxngjizv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3jbegaqsh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3flmmmdtb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ibgciaai.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lviehcnr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ichtkqmj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3kjhkjyrx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3odpdvyoz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3qldnmtiq.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ofhzsbss.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3frnlkuhh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3uchqddtb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3djdqsbvu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3prinmckx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ffgufkuw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3dnfppeim.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3crjajdqw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3zzpoubal.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3qvunrwwf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3lbqqxseh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3angandqb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3jtzfsgzv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3lyvgmoaa.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3quzkimmd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3wpysessg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3owezavfh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ltxwbphp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ejbghbvy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3bnffukub.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3bbpbqvfo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3jxzzvhlk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ygjpqjxl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3qqdvfnum.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3gfygwtcm.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3kmtuespu.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3rsuvrwha.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ptwhbuui.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3eekvwnga.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3wonyatdr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3rvixbocl.html


<!-- 参考信息 -->