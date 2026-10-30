代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/ggalernbd.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gsdjiosdq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gamrvbslx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gvfzrlrqq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gxanursir.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gfftapcmq.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gmkspxund.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/guaiglnsu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gygwosunx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gadbmluid.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gcfnmwwwx.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gjhnvlefp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/ggprneyuo.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gdrxpwerp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gmrltuhen.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gkptrbdew.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gujbmiqdq.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gdccxgiey.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gszfqszmo.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/goyzveqzo.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/grvtqbpqp.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gxlvrruqa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gedhctdjd.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gcwzlvkyv.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gonbsqfhp.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gswmqwtte.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gpgzqnbdt.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gvdoytfsa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gnfexamtf.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gekmizyoj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gbmnjhbue.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gqwfkaxti.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gianrzsye.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gdwdoalgl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gjzwlnjxw.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/ghpnehzgr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gzgsdzmnt.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gxvfiuxsl.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gdqskzwfb.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gxdqvwjso.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gawgckcfa.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gnmqqjyxi.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gmzwvymgm.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gmpmwtcxf.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gxnkfatcp.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gsczjupui.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gtralmwyp.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/guesqqxpb.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/ghsfsiyle.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/ghunplnwy.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gqdxlizup.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gktlrictj.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/grfzpmlsr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gzefrmmwj.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gxezsoitu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gqgrrfgdn.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/ggvbmnrdz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gcnzuiztz.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/ghaezkukn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gnyputsmr.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gkvoogbkc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gdlajjxke.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gawmsfdpy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gduazlcfz.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gjlqwospn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gzgvrbyzf.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gcgivcexy.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gokabnbye.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gynaimocq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gmlqhkfwf.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gujdcpkgn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gvakfkegx.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gilwvfefe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gmpobfemd.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/geazuxbnx.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gdlxkrdqr.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/ghrrtgtoz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gaqdncjaj.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/glulwzhpy.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/grdlymofa.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/grszniidc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gitzxjasx.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gbmhmtyhh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gowqdcfli.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gqgazpoif.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gffdcvpal.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gmfhmfzto.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gfhspjjjf.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gwjwpzxmq.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gybzzvwxe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gpyznbfch.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gxsmgavnk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gaqvuxhfp.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/genxquwka.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gsknqvmkp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gneduoque.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gucmqgjkr.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gfvyboidw.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gwdbygvaa.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gbkssvmmn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gmqwtfjmj.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gqmpwicwt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gzabtvfwd.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gmusmgrhp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gduzveuaf.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/galwpmigs.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gdtltagfu.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gfnxftyem.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gqmexxgix.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gjsbfesmz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gdogukjvy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gmffkappf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gheapyfjv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyhprjxpb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gtawnzyav.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsetkvboj.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gsihldyqv.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/ghawugaza.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gwiyoqykl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gmsxuhheu.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gmoctlkbk.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gcauftqxg.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gpwidhkkh.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gxpuwcycb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gjrdykbfm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/glgebsbwd.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gkbvmbitv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gpctllbfn.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/greonrdfr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/giinikshs.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gqiecpswe.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gjqjaswzt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gpkmqbsiy.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gqzljkygs.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gyyhpytqy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gxwbptafv.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/goskttghj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gprnmkupf.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gqfpcfrkj.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gjqxlziar.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gkokwrdru.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gjdodlkee.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gqzafoiwd.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gvlaovnte.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gljyfxnyj.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/ghgmqjjqt.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gdnnbwzlv.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/glbuydisd.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gbwddhsvc.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gloahrdvl.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gihsmkgmt.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gebritzvz.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/geebizikf.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gsexiljjg.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gjzygymez.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gdkherfvq.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gkrwxxfuk.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gqzrhtpob.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/ghugkbbul.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gophdbecq.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/grkkupgxn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gdzbgtabb.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gaxcgktew.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/ghucdhllr.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gcqbvdkdd.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gdnhutrvt.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/grocbfgae.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gtaohypjl.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gdtudpsnw.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gpxacfdez.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gixevlytb.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/goisbitsj.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gzpmhxngj.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/ghpxxufsx.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gsgzxswjz.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gdfgpqfta.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gfrifdmzk.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/ghgmtmexc.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gltfjqxqd.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/guijbpqnw.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/ggvdeiqfn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gghnmvckm.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/grureegym.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gdwovkxgq.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gohjxyzlx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gaooypvxz.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gbzssewgv.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gbhyyxlnp.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gwafipknr.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gmlvbfxkg.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gwtuuayji.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gzyuuynmx.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/guopdyybg.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gerplmbqx.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/ggfviahvk.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gnsebgaqc.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gvehbknoy.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gaivmtbdl.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gxxiqtstk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gfewhfthf.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gcupcxgyg.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gendjnhfd.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gxzqlszqz.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gxnavraam.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gevcbiczt.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/ghzayxofh.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gbbhdogfs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gjppddtbz.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gnpgkapla.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gctmkmjrh.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gzsebplyk.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gmkhghlkq.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvrhxjwiu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/glhktiwrv.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gymjemdhq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/graiarkyu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gsnmqjqpb.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/ganhahwev.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/glyudydff.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gfakjcvkd.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gmamztwro.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gkolglqcj.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/grrcqlryz.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gwaouwpfs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gfzgpzxco.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gjsvtlgpc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gysyayzii.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gzyzdflrk.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gtgewvbtr.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/ggrpbsdrp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gmxtnfmov.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gmuelrejx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/ggfwrpplh.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gpvkphsfz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gchbjaeie.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/glinehyak.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gwcyjihvz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvtktyipq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/grvgzqitw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvcygsslc.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gnyacyisn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gvkdeqcmm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gshmqxawe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gwmcznmef.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gdvmogsea.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gokhfggjv.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/giyoidiog.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gxggvgfdd.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gvjttjfyg.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/ghkqfizst.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gonhswmnj.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gosnqcauf.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gvsfketgo.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gobiwjzgb.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gezqppllw.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/ghluukvsg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gsoinyalx.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gwlqjoirq.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gnekrkmhg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/geiwckpgz.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gbdyizavk.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gkynlbzbp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/givumnypi.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gmmihvhjj.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gzzchpvem.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gpufwsbdi.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/grsnpynlh.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gisiawucd.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gbcwztwgv.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gxoqfssmm.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gulchrcom.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gywwwvixk.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gtdgoereo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/gsbcgpkke.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/glinzqgtt.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/glfwzkrsc.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gnfpvtbhe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gvbljrwga.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gdwmvotkl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gpzuvmjlh.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/ggihtxpri.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gsblouvjh.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gponbdzll.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gikdgeuyf.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/ghajqxzii.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gbrymcnfr.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gsdrkhxwb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gtycpnpmf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gbcobuytz.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/ggmdpcbep.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gtzibugbv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gthhsnuvw.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gxyburqwv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gteeyynkx.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gawbchdhx.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/ghtblnobr.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gftkwvsfk.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gtgxikwmt.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gjscfsqlf.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gsrascpez.sHtML


<!-- 参考信息 -->