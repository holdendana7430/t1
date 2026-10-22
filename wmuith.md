代发 wailian999

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2niliwlqj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2tdyzlulq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2srodptnh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jvkojulh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wihcjjhx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ksrjbwwl.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2fqxupobv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ggvoqxxk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2talphrle.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zxcmjiad.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xyqzoxor.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2jxwlrpfk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2flnephei.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2uygdoavz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2psldgrzu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jhlgapln.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2lxxkmpyr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2neqbwxau.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xqsmfmti.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fmpzeyoa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xmqbyxoo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2letzdrtn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2tqllxigo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2whzwdiys.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2quykxdvn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lrietssn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2gdeqarih.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ftwbcxuf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2rbrdgosx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kvobsovo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2mgpxtray.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2tctfubsc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2hxwmsuni.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2dgqoqexh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qpqdfjoh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2orustdnb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vqmjnkxt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xuiatqcv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ruhvqtkf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lgppwhli.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2hohqlauz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2nxjygvpg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cjnsdgwq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2pgtbwqpc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2znxlhzlb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2qjalbnhw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2bipflbez.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2nvoecvxw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qgsvelzm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2fvwjcaca.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2odnbvdvi.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2fapcdtwr.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2obxqktdh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2mqahuotj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2kbllvjik.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2vbrzetzt.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ionqrrma.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2aknqnwjb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ctigmwom.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sgdnrydu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2naoohsmf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ngkkhycd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aaolelhm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2kthbcocu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2dvxtjczc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2wlpybtie.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2czxukvdj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2iafactjz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ddxaivim.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2heginski.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vzmmxzrq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kfhnjpyr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2yfmmphjs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qvuxffpm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2dzrzphnp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mzyhygmp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ofunssil.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2mbpijvqp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ltehkawt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ixknmdgl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2webzdxeu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2vludqmps.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2feqkyaif.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2tqbekhvh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2aasfenbi.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2suqtwlyy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2elfkmebw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbjnshmw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2gdaarzhv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2iuxkzgjb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2fyxwxkdx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pnwzhgaa.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tqkrojtk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2pihneadl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dxjygqox.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2rpscckhb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2uchzbjfu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nrxrdyhk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bicazujs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ndlaakrs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wcgcnvvi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wxajdted.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2yhuluzyd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2wewopmoa.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ikrhrxbc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ysrhaffm.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ycbqizgx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2vufkcmcj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wramzcox.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qhguubpw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xympkvno.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2imaqyjqs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2kemcgcqr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2wysfxkpc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mmrnqfja.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ojqycmbz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2nvlzcbai.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2jfxgyald.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2cbxzebip.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rnimnhii.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yhdylxzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yttcgnto.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2lutpbgxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipjxnpjx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cxhabeov.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hmceuptq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2mzwhgksd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qeiptfgx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2sdhfvixw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lodbbnph.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2cccorkrb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2tnzkqqrd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2srusrnjs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2oaxjfdqx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mriibvjr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pdqznpgz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yocbysom.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2oqmseczc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2gqwqffvz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2aawvbmwl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2kvjtktya.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2abxwdbuw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2zdwwwcxp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2nafherzb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2hybsojpl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2sknzojfh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2hthotupi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2imipwwxm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ucpwpiez.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uhgixbby.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2xrjuhctf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hnoncphe.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2gmxumgqc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ojdtoacj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cmbevfwm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ctictqjf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2bifekcbo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tygftoae.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gjdktiqk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2dgtnwbld.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ymgfogwg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2byopuqex.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2jycghpgc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hazjbehl.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xdniopgj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2mdbhsesy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2qocduwvw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2itfmfifq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2krizapdb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2abjkoris.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jxlvmngh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nmwmochy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2footgnyr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2uupojhae.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2cqphuoqr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qptlibjt.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2siqsegpi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ubowpdwv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2copexbho.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2osiigbno.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2gspyyham.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mermpbos.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2thppawji.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2mksqgbal.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xdqjctui.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xedhvubz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pgqsxtkn.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2cpygjbkb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2plykyyup.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2wnpmvzss.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2jvnuqelb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2yvlyzhim.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rwkjqgkb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rcllyfwm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2sltwmune.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2tnkvsdjt.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2zvribooh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2pivjvimr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2zadylgzu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2flwqwhcc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dyojyixk.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dfsmhexu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2rfzlolrs.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2bmohtiqu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2effbedqb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qzbbwjfx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2evtkfmgc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2yjjirwcm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zmqnjbos.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2maqcuxzp.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rdhhgyfu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2izcoemxr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tndvpxor.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghxvwbqp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2agxssjiy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsvizqys.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2osqkgbbc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2cguctsgj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gajnvgpe.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2yavhvprx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2dytksvqj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtkmcfne.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2avenihwt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2gsrmikpq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2torhwwns.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fusluubt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ryxmdqrz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2annnnneb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qxjrkrth.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ivtutisr.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qtuvutbs.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2qpqymqwd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ttugyevd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kubtmqsp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nykqqckm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2lnovimwc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kxktmncv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2exkuhxlq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2igiddxrt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2aaeadjeh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2jqhmprqd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2tujstakz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jqklfcew.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2tkxpumhj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2anotyvmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzecwgjr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2reulfexd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eqqobvhj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2vsqkwcqp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2zushgpcr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2wupwykoh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2htglnyov.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2uqsbsujp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2xaisjovs.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2aoprifnb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2hbgpwdsh.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2awgyqmpk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2oxcmukzn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2tdppdtqj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2kkdftalf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2eycdnylm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2qpxpfqfn.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2xyehogyl.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2exroxkrb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2qmvmtnwk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2izyygjgx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2syaolswm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2thaoorqf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vxhaikdy.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2yroinpkc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ukgqnjpn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2llnkfkhm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2zuauljwj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2jehlxgab.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2smlqwxku.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2obhxtjsg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2gfhdzzae.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2odsdjfjz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ejgemfxk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2dcyelztj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2bctinwfh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2unghbwmq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2kqcgootp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kceoqdmq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2csxdedss.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2oqnfjdxi.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2mkutcwto.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lgegddaa.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2mxzufium.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ndrugbvd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ftvbaexh.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2kirqhfsm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2finsozto.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2xozarwmm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ffalzsxq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hqogcimm.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2cfoymknr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ygoxvbxd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2papztxgz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2bkbzivlq.html


<!-- 参考信息 -->