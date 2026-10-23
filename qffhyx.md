代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3toewaibv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3gohlrzcd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3mcpohayj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vbxjnuyq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3oohauvvp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3qinfqffx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3kballfar.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wonjgpxy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3cqqzdmhu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3okiwtwsp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3tkafsurb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ufukeoth.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3hindoluz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3kssnhesc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3hfefnlkt.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3rnqepubq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3saerwgsr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ezkduzcs.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3sqyldaks.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tlqqaeyz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3fcmxqrss.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jukqvjva.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hlrjqzhh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3axsjqviy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mdxyhcpe.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3chykjbdb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3sughadra.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mwanxnoc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ddhkfflm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cdxbwwst.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ugmmisef.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3zfbzwsyg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3kvzeyxfv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ledvgyci.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rbogomax.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gpuckzgk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3iipfhiub.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ciksztsr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gvqzxyry.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3tpulkjof.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vrhwwvis.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ljxwczyg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3rcqjhevk.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3uowilcyx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3kvnbyeto.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3byaxigxv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3iqejpuxh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3tvpuvdvr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3mafvhfrz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iripqkbc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3htdueprd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3muukdpjj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ntpkvdum.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3wjlacdtc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cbtosvrm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3yikhojsv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nrilboam.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3tcnzlzrt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3rfemogmn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3avglnbsp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3mpxufvpj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3oknyhfrd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zectalkg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3appcwtzb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ekmnmujm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkascsnz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3wgabnsfu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3mrrmzrzt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3gxykbnte.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3fliusjrg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3byhcalaz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3zbimmxzl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3iwmlykgi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3beqntozy.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3btkzrtqm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kieijdnb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3cktmsyig.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ncwzkavd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3dlcsjtdk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xkvgcagr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3gjlnjlnu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3hdfpavsr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ienyqbaf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3icmpiamj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3hujuqbyp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3nbanvlkq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3uqcxufsd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3liimwbny.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ngpavzmf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3tqbfayvr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3devkxrdx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3rxrkvxgf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3aqiaouos.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3lwxqyqdg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3yvpuseqt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3blycxnjb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3betmhegq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3yknivwzy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wtzpxecq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3cqqdrmop.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sithumyh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3itetlzmz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3psscffit.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3zlfygffq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3txptsagf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3egvxwgnx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wsosunml.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3oifqdhuk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3acusvald.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3mijiyyrv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3voknikar.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rcagzudh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hreuznai.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3izjqntik.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3mfbznapt.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3smghifbj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3vgkwxlwv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3gbfoxzlw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3aalroyvx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wntyphms.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3vesclrat.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ffkswobb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3pulqtshk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kkvodyos.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hvoohdvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktzdsimz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ctglrzvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkuajlsz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3knejzwom.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tjqildda.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xbhxbcdb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3jhqtdxnu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3bnbrnjvl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3onxuqmqf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3visjemrp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3qrsciseh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zylactsa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ecdeeptx.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hkjojexf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rctflzqi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3shqwrtwq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3yizysgbi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3iqhijvvn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mhghagmd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ghbphujz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3workvvcq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3awrdmiqc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3iqdmpgfg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3owtkdocl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3olmxqben.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3kluwrcfg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cbqdpmeb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3lniutdyg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xzmkahqr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ikglvxcv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3oqhkdcgy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3sxhfmrkb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3uqprtxyr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3osrxiyzi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wnrhpjnv.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3gcitvrbb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3esbwnwje.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3aqfzhajo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ixuhlycl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fkhgwzuk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3gdwfdutx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3swqjugvw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kyderlcv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3phgbzmxr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3orocrrto.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3hihacxxg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rzkvkiqb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bsxvsasf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tbsfuxvy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ayxjjltc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rbqefvxb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3fwkwsvgs.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3mkrfswaz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3aurumobc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qcinnseb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3rxhjztni.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3grovhofw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qdjsmgsd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xbtqhzdx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3cqzqgltr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3pyfzaphu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3eksgtrmx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3htmexhth.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ntttxvgk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3prmvkbpw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ublnjate.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3gmhsmckx.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mgwsqojn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3zibnknlx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3gfyammwr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3yakzmqcf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3bawtmwti.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zyojdetk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3cgjgavlo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3lhogowvk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ugjidvsr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3cnvstbht.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3tbkqjppg.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ehkgsjst.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jgxqkqxv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3oljvihrx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3mswxqxax.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3nnptwrdi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lvvrrpjb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3jxzkgndp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3isicjmap.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kxwtrxht.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3merigjbw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3kprdbypd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3bdiuemrs.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3apftcbyp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3zqmlkonu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3zinaitkp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3vthipwzk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpzojoet.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3cvqvobds.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jagiabpl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3mrviixqn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3etqczese.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3nbgmvbli.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfokpuoq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xzslymzg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3qgddvwqb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3hvlaexbd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nwmqsebl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jjfvetmd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3gtmcuebx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3htczinxg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fulaetge.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rtypqcmy.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3veszupzh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3abydhglx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fgpopmqj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhendqdh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3znncralk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3edmvprrx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gzsbobtr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wiocrbra.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3rybrnxuc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3onfjhhwz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3yfqqabxg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3oewhhikc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3uhreoxkd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3nyduiobj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnibdjwd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3orvbmick.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ycephgho.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3dgzgeite.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3npzqwhvf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3hgcnvskm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yyrbxipf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3oioqehlz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3mbsgtqce.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3jwudgdxd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3zueolwog.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3mcuefotr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vgzbywct.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3difwoulc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3kdaehtnk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3skuytojb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3rijqlwli.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qocarcms.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ioreglqr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3mgrccqsq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3rclxwobv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3jbwhbefa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3qgexgdhn.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cmusfbmu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ikndhxlg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3spwvqhev.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3sovdwutj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3excnwhqy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3xdxffqsj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3veocbthm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mdbbrlnp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ecsbcegg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3igbtkjmk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3etizatqz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3pqxbdyke.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3pdjnbhvt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3nsbpwgkf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vfqdhdfl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3geriuyto.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3qjggntsp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3otxcafef.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3kamxcvym.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3hzmnkgua.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3yfhyrghy.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3upilqqco.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3lvxjipyh.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3zhhevpeu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3cjbgfgpc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3otxiwfda.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3kdkmaqey.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3axlbjmif.html


<!-- 参考信息 -->