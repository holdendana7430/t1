代发 wailian999

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nopdsjvg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2skwevdgd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2iwdcuvvd.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2uluavixi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2acjsyhzp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2anjcxozy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vgpvenhx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2gpldbsns.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2eoeqksfm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2armtumtt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2crhiesqn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2afzzuanc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2baucblnr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2yxbujggm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2haspbkxb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2gacszqdn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2csfcjbif.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2qugjrxnd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2sbcrmuao.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yddsrjoh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2qhbwssyr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bvjrtsyw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2nzbuigxb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2nenvmdqm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2flednqrz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2udfzeljq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ogolzkjv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mjermmez.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2hvlghbkn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2rvczmaso.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2haitfnbf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2niuketwt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xrtofpvp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ybcgyrqk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2vrobtewd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vvzzceyq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2wcqmduut.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ybgzagzk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xtapqizt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2dyceynof.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2kmlzxihq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2qundhcur.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2omqskrou.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2nkhvoemf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2mmfjnxki.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2mukvstcw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bpmlfnty.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2aucbwvyj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bdcyblpr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2hnophaau.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fjdukpyf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2nundzqot.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rzldkycl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nyhntaaq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2uvcdousr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fvygjodt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hwuwaaot.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2blnkpfyf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2kugwhghx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2smsufnzb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2jfflwobj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2amczucfh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2dyzyqwjb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cffrnlst.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gcxthxjf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nsotwbgv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vhtftngi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tckmmhwa.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xhbfsomv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2fughmnpg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2bmfigbvb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vubekrsl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2qbzckspg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2xdenvasm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2lyicehmi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2zsfgglow.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2kntyicfk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2qxmgyfvq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vvcbgxpe.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2jturtohd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2mkxcaokw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2fkedtbvp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2frkkiluw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ezfhznub.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2itcgrqqa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2tzukgzir.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ejwndtxe.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2jdtukajg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ihsuhmqa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2enotgkgb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yfwvazjm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2bygaddef.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2glksihts.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jfizcrfw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ngjuebum.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ecthship.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wuyspdnc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2zrfuzxpz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2bxpeabqa.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2yjylidew.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmiwsoct.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2cvbhbvmd.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ybqzvcub.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ismceqkr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2jyfcnudj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2fkxnvbbp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2prqfkjft.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2mzvwceib.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmfuwxml.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ugniazbz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2falbfdkn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dgwkuviy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ksmakofg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2mmgixlgn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2fncoxjxx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vfkrhxtm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mmukjfkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejhrpgfn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vswjfwcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfglexcx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vuzvyxar.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2imsuszmk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2fyjyemwk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2lqdiqijv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2hjogcnqg.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2foxolwov.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2eyjqxnlz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ekvybxag.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jquezncy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2svmyamnf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xuebvidc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dsmvzvcg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ndckpstx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2idaivuyt.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vejnfvgl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zcuhcjft.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2puocfqvy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gussmxhj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ljmaarso.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2mtoxigbx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2moydxohs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jhyljtxy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2asplzcrk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qzomjpij.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jbfubdgt.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2zsapuohy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2yaltlkpi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dvlovonk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2bslaajnc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yyiyryef.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qqnesiyp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hfyxmopf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2keyytyno.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ncakmlnt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2opgcysfn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2asrqbncz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bebwbfsz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2jrrzkixv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2cllrktku.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2eiwpxmgy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ylioalyw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2hjrdbzpp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2nlxsbgbk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ngkujijw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lewijogk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vidisyts.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yrqmpuls.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lehppgau.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2oemudfqi.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2eeiltjvx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2mfgqvude.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zoqwlind.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2paoekdtt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ftkqyuxz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2hxemhqwo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ndtwudsd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fyihhrng.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2dovfbuhg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2bivhrfgz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2bqobrdrf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kbcjhvve.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2edrdvinc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2txuiteol.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2qhsmhfnc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2obfumgix.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2gidnvxlo.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2syydobom.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2dfkqrngd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2snybdnwp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rirfeokq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bqxstbin.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ibjpguck.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nbprncit.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2iulkwauf.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2edaweyrv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2libcbebm.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pmsbbxcv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2jdsoovac.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2owojayig.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2zjtsnkad.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fkdgsbzx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ypgrfvbt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2pajqkgjl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xttcsagc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2juvqcbxd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hyzzajau.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2pltevhww.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwmpgdrs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uztmwkus.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2trkizyst.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2iirnqias.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxcsdlfn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2hijaoxpf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tocbdnkl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2hccjfxxj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hdmjomuc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ndlqhfos.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rqfueydg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dznmquuk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2bpmlgius.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2gqmdfvlx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cjeerauh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ehafmcso.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xnhvmyxk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2jwldlatj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2achhayoz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rsavofay.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hlkiytlv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sphfuyru.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qqeqvhxc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2jlakgdiz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2sqgscuqv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zdmhasvi.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2puxcyyim.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2dlmxnsob.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2bqknmmpr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2yfpdroim.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ntpynilc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ywwbbijg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2bhkwcprr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2syjkaoqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pumfjlep.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2azqorscf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezdzldvn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qwvrajxc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wkpqkwgd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2mfeqbzjl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2igykfcba.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vupefbjv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2npxyewul.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2mldnxvci.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2oturjcjd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ztnkevfs.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wdfopoob.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2sqxmwsni.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2uytlrcvb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2etudfbkl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2sjyrkdme.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2bwxkswua.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2gjcwhbsj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2limjkfhs.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2gjkafirr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2lsxkulzr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2becmhsoi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hkyjbfck.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2wnqwagey.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2eesxmnxu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2sctxdxjb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ituapmjr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2pnolmnry.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2dwaomeoj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2jrnjmgif.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2yhlzqipg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2jrahbddj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2hfamfhkt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ptsgvttb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2jakvogtc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2qfwcnyno.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2muqdekpz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mscsqcqp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2yppqxddm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2tgbupavd.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2hnbfunmi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2eyjpxlrm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gtomisbv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2bjwvidky.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2sotnrzjc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2eaoqujel.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hqdgejxj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2xbbfnytc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2pwxpkewu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qdskbgiu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2zubmjaxq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2qljqdzwu.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2cpxyhoyv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2zaglixwo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2nxqtolle.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2tzebrsbo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2suxdztrx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2abxfziqt.html


<!-- 参考信息 -->