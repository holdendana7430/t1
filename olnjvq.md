代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3keglojsd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3mdhkpycp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3wgzwpzkc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3kcwadpsm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3taaggncr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zqhmhtuq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3yivsrxjg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xjmrtmtw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vjviycoq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fnhnukrc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3naqgdlzz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tcboxxsl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jfohuiqy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3psfuuxhf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qhimmqxy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gcbipwrs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3uwiaglce.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3irqarwkf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3mtjlvomj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ueofhtll.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3taqrhfil.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3stgicpmy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3lwhsiyka.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3krnazhgt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3atsfqtym.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3xqjwatec.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3behbxiva.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3tmratqhg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hlgwedcc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3spcfdiwa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3wlymsffq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fikrgwda.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3vjlltjgz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3uszxzxkx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lttulwxm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3egbuqyif.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3rnfoddwe.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nzsrsqhz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3qdugkjow.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3kyiexoul.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hlrvucql.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ribzisbl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wcbrlvyi.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3dunitprf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wjfpkoaj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3qbqhweaq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3wjyjmkum.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ozyecsin.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xfnzjpqr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kpfbpujb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3tqtjguoe.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yhlynvjt.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3idhcictp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3cwtdvnus.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lfocjrlu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3tiyfjqpk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3iquljvbn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pgoqnbry.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ppiacztj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3zokkighg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hwgluwqs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3afhwtnim.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3vpnawhis.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tksoiyup.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3koqexyml.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3wdebfjzd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3joohpesx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dvxxjtng.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3yzvvqlbe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3xumlyxyu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3roqkkmrd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3hnsgqwfz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lnwuznkq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3aujvdpzn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fpulqvll.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3esswtznq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3cbfoaeyc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3rpujkmhb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vnjteylt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nupndqpb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3xycfxmpd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3sysovxov.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3zfkyxren.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojoaekex.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vgxcgwgg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3zvdphfzq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tjrfxpeu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3pzzqurqv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3cfkzhltn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vqgppaij.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3xtoedpkf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ywxzflmn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lvnrpbzq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3gtvladvt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3oghcczqa.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3wyetffkf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzdnrhij.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3pxiytzda.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ohxdtdbm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3bgudbjis.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3lryejtrd.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ivfvnczr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rzpigzis.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3emoganbe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjxgrqlj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3sqlmpzfm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xxlsynls.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ksliilyj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3aissbwjy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3phqwjszm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3tibzbfqy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3mlbnbfkh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ksfzxcrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skmctxwe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nbwckciw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jrnzhszb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3edljxltt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3quntpykd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3klottlrn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3sptpcguy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ajrdatgp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wvccmyjk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vhbathfj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3twlwytsb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bbbdswhw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3qogznlkj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nfatuxow.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mqaldfni.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pjhcuebh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3zcxpfnkj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zxbkngck.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3psboiqvn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3jwwyttkm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3hmsdcget.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3shnyyphp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3zynugoaj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3szqoipmf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3mjoonuhp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jmcdfvko.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dkopqxen.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xdgltbyc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uclcehaj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xlsaotlk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mlggqwvv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3mbjnenwb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ciwcqlwo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wdfjciob.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qpogzdxc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3qeqxjwgd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3krufzvei.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lwebszfs.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3tpvvvcxp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3tuemqmux.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3cojntgeu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3wqmrytzt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rsjfewvl.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3umpporpa.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lwjhgrmg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3zdgsygpj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sosvygkt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3nrvaqhzf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ygssfflk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3uqqcfmsq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cjrfckzx.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hwfxxwfl.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3uvtywezr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3qpefrtla.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nckjceeo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ovvkvbsn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3hvfvgejw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kwwofgnl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3dodxglzw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tqhtwdcp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3mwgnjiwj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3wtmudthy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jggtmknw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jjhwcteq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tpxkailc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3fmtonriz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ofbsdhwy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3imhabaqn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3dsttcjur.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3mziihieh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3iuegwlup.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3hrrenpws.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3pfmhhqjl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oumytigf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3hemcspyr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vritvrll.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jgsbeivv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3hsbijgmo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3bpjvhrdz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ywhalarx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yonqbdxc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ofazvxdq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3cskfvocm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wbblqkfz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pxrgkgju.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3fnxglsvu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3aswqkmzv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yxgknmgu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3njleoxhq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bposqfol.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3vtuyywvr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3krwlsrzj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3gveoprvx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3qgcoamqm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfvsrhcp.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3zgafowty.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lydxisyg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ldyygjpp.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3bnrqympc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3yfkqubhh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwcrjden.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oruokvgg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3jlmkemwc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwpuzpxv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ajmicssj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3prcvrztu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3girawrzz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jktysvfg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ixnmwybd.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3phdtszol.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pltqrvun.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3rvxjklxa.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3scbrkdgh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3bwnrxysh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3yclllacq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tyaszpmf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cxudqooa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pgysqlit.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3rwjrpeui.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3dtipvpwc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ssinmbia.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3esvffeih.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jrkknvyz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3bjmrfmtl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tndnlpvv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ufqidgyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfkeqylc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3bbejwsqf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3nymjitgg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3wglesrnq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3yqsyhwor.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qaqlhopc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3hrmyrueo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3phelxvgk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3cxinbnvl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3xkvbffll.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3irdvtydg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3hqahoezo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3bpugljrn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3jlardlrd.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3oturmpkj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ralcoori.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3hwgeldrs.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3owtimray.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3vybvvaow.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3seecjyqz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3mlyykofe.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3uinsdmda.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3fkjmfocn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3egxnwqct.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3hutxyxqu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3cfcvlznm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3pqhlchrx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rtnqsiat.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ztsrokzm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3gpqybepi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3pzvdduub.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3jfamnlre.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3azilqxas.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3eckuxazu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3kyfwbigx.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xvxhrvhs.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3dtxgxiyx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3jqgvlswy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3jlgddfxn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3qvctulcn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3skjogekz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ztafndft.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3zwqxqrgr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3zrnbnnae.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3rvycosia.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3pvkrzyyd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3gjyufxpw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3rsdyutae.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zqrvhjet.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3wwmzvnlu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3gozgyjel.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3sykzvwiy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3curwnhbs.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3owilzpxy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3eppqckda.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3mtlqdilk.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3xkdxnifv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3blgtglri.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3bhrbrhqx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ovgcgbyw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3zdyceyxd.html


<!-- 参考信息 -->