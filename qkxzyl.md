代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2uqnvpque.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2jwqgcdib.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ngjfqcxy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2tockyrru.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2xnyvnich.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2lnmerajk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dqlnjjkn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ohtjigsr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2tmzzouiz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2diipeeii.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yqmuoama.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2bpedgimf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2lxllifnc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ffshhuew.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2lmdrnljs.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ypnbcjzy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zfxidabn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2lftgrofl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wpzoemcp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2rfoxvaso.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gvhfrjol.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2naethcvz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ppuopzvb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zixgicxc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2bzqvfcos.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2guevgtgd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lvdblqgv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2jessbfnx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vqkhveey.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2jkohtcwf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2dawbpxny.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wyrsdgbo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2lqidrexn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2puzumxdu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ukdoopxq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2wcyirsna.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ttrptkbk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2kbhvuzhw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ydbaendh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ozlglpxa.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zzraflef.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2cqiynvmq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uefpxztc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2uyozfbuc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2uuarcckx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qyrzgumw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2cpzleban.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2giemcwrb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2yhbakdlp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hqtzjomi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2iwoqtnzo.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ghdhxbns.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2egjznxog.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2tawrvdcr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jznnnrsn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2pkjvnkwo.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ybrmhyin.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tkatjgcf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2djjxnoxq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2atszuxrg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2yykbddeo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ayegdtox.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2wxdjhwkb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zrbexyem.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2tnoxqkqi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2zjyjibxv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vzsahsne.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2usvwxgbx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2yqrevrns.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2useznobj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2nvcipnnj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rgxwvboe.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ahqnriva.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2gqzjwndm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vlywkjku.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2nbosneej.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2zxljhudo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hyjahukj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2vjqtcdmf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2nrqwxgkf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gnlbtmkv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2timlbofq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2rhgamhrw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ueycehdr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2oxusdweu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ztyuyvlt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2opbtumfh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2zjcfatkd.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fbdeujat.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wraorrdb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jnwlsrej.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2eidkltoh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pcpurcnd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bddortjk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2cfvuojyh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2dgboemte.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2oytjyxkq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2cgmtovtc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2tsrqdlff.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2pyslektk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2pgcdgaze.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2uvxapelv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uywhwhav.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2rjhafhpp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2balivdrz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2albpxbgg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2jlqojgyk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2laaqrebz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2azkqbyye.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2iaxcgbvr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2xlkbjiox.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2gvgmxakn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2btlxmwee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdhqieta.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2pfgisqyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ifzchqss.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2otypcnrq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xvmgzkzq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nkxbttyn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ilcxmvnv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2rsesumkb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2upavbqgb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zdgrqxtu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wfbybyrb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2zqtncsqq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2coaageks.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2saqziyip.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wzdfpzdv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2aknkgali.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2dskalkfz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2sftepedu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ecawlhfo.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2yojvauoi.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2dqinpumr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2dfkmndsv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2fdtomkjc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ynsincri.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2rseymhcu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2zclmdopf.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cbusefgm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hncdtvhc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2adlarmpu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qmwiocgy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lkbiekul.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2hrtxpnyd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2jfpjyssj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cmdmcjzh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2orsuppoz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2qwrgrhyu.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2cpytuzff.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wubimmtt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2rzprlndl.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2sdwapyxw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2jumejtjq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2vrezwujc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dxgihwxw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aezcquja.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2kwyipeuq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2iulqywlt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2vejoweql.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2upnqzrww.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qmeucpye.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lmjtwqzl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fvlfxbmz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2aqwceibx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2dokiownp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2voahvufi.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2bvzsfnjq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dfdlazij.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2oqwdyphq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zatkzfvo.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2bflstjoe.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2dfqijwvf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2mwpuaxyz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2tigbtlfa.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2avqbudhw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fawfoecp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2raphacww.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ikxkfvjv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2rhmezeio.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2itubyfhw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2xogtpdzk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2bmfsmuoq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2wdlvqrca.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2qlcchnsn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2uznjagcy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2syosjzeu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2xltsqlzn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jfgqnggw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2yfeqifyu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fwxgqjqh.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2wwipewhx.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kwoyfkux.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nomfobex.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2euugihhx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2geunddtl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kwnhsgoz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nlarkswa.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2dewenejq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2flmzyvwk.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pvhorqsx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2vmvmioaw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2soojjzxh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvauodms.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2hlmredme.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvsuhspt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2zbotdcma.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxolzhbl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2bcktexmv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2roymttwb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2rqdzyvri.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2gnzeozmi.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ntddszmd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppkqturo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2szbtsqqk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2fjmwjnkm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2brxyghei.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zqsnqniw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wvapyieb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fqjkjldm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2izgxtigr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2acyrczno.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2csswxbho.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gctbuqjc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ukpgmhia.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ezavmhcp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2rtmhdcuf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2jmkjinud.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vfikqqhy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hcyegvhz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zpffhtgt.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2clvlgqrb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hvdbmcyy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2kiiqtani.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2atgnxkwr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2zooziyyz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2kbqhnwkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xqfkhrbc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2obugyejz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vrgecoxw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2eyxdaglx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ptczfacb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2rsgroywr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2uygltklw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2flqtmtuc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ldlqaxkf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2mytfwzrw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2tagasclk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2eqbhcurj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qrfhvjao.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2enuyxrfe.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2kstxjubr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kpwruubn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2pruvyeqz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2xsmnaaoh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2istnortc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2kowyrmdc.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2vskaegoj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2clwukngl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2hpfaekmk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tprazior.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2uaexseoc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2wnibkmmw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2mjuptrjg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2aszegeys.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2uxszqzyt.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ziremrzt.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ywskqkhe.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ommnkpss.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2xngibqlf.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2mbwsujpd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2fthdwano.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2imkwcurz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2zskknwal.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2rhhybxhg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2fsgiaapb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2srsejgvc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2kekmglwf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ugbnhsva.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2senommbi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2trgrqbfj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2xwsrgauf.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ludbptgt.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ovnauenm.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2nyegqcyc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2jjuwhklu.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2aupwdxcv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tmnwivpt.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2wtwumjsf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2tlkhvbqf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2wmqaisfr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2iyusixdl.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2zbacgaji.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2amsssbdm.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2rttzgqsg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2hjhwxyjz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2xjtnqlww.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2shahoqad.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2tkkcftjx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iagcarrf.html


<!-- 参考信息 -->