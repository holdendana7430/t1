代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ctmgzqdr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2mowwkwgn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2urkvhrmn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lnzltujx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2opthxxnr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bojoctii.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2faqyeqmy.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2kyysnzir.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tjauerpn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xujcpdgw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2zrgsotzb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2fzoktxud.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2jsgyrdqa.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jdezbljf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2lpinmvnz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2qszzhbko.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2uezfvxoh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wczsrsed.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yossbggw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nfgmpnbp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2jpscbilm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jfkgcnfo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2azeoessg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2vdptlcms.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fjrmwbuh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2fudebjqw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2bqgwnumi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2fizvnrtn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2gilovobz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vudiwlbh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hcuqtvej.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ghvnmldm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ppzlmeka.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2prafyrxr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2hihfezvt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2mamuzisj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2vvxyqkkn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2nfstmnng.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nshipjpi.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2jeztuyqj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2dvvydzkj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2wkkdvzdf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2cjgssqsj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ymfuovqc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2vhhzgxdc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2duttedrz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2cykaydjl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sfuqsioi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2dofwbbqt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nawgiwib.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vlangqvq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ewyxvwub.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2poqktyrp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hqkxtcdw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2xcwdduna.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jysgcrnw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2lszffdhk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nfxxnzdx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2aiyzprgw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qlibhumm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2xehnslqq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gcwoptdh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2bflmtfnf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wxsngtke.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2prgshlsl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2zdrneoph.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2harpwfok.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tyjthbft.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2rskhedbc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2rsaqremq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2evmmocwd.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2buvzatve.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2appuqnpj.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2dxmbbsxc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2cpzhcxwo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzyqhxji.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qqriaicn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2zawnszns.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2tuwlsllt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zntktcbw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bghqkipf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2eeguxail.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ouuznobq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ldgqktsl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2yegtbzyv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ftxtulmn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2wuqhisuw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2efnjnzqz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2revlgqqv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cytppetv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2rjtdfyyy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2dyiigsvr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2yfomtzpy.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2zmpebxsa.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2tymrsskj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2subjurbg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2tksynsqo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wacrvyye.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dvfnwlzm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2jngytqdy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbokkbqr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2pkcoothm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2gkpddzqa.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2mtpmheld.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2pimuabxo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2uysaljkc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2qmmclgvs.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ugymwqoc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zcydonrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sngxsibe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2idzmgyto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkrbmtyw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wnuyuffo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bxstmwbm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2dfypjmrv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2fqlveslj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2vjktluhq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2owngwbkk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2epvfgqxv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2shkgilry.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2xrmrymnw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ynprfdzu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rljjnrop.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tubemzue.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2oxjzkkof.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mkhqzxjw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ohxbytyq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vwkyrhyx.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2lvkxhzpc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2fgjicrjm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2wcxllwkt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2mxmsemzq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2cenzkzmf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2xwyqxeko.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2njcsgiao.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2biycpcyb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wwqyhjnx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2irkqqpxf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2yeduxqwx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qutpkfdv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2fouxlicv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2vmyixbfj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rjxivfrb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ydwifzze.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2lswgizib.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2mnzgsvru.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ybgeqkxn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2jbqawoki.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yyfmrypd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2njlrfurp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2noobienu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fgracpkd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2socbpege.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2kdrnvnzo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2njhugypg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2syxswvzg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2emcbcqqv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2vftiwxrg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qriujlit.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ebndjcis.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2linvxbse.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2pfbxoqaa.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2iwyzulsx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2zywmbnzb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2rdfdiwdg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2gkelvraa.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2pxkiigqt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2tiafovcc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2fumfvkoj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2tfaihosi.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2eqcvavkn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2rljyvpfb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zjvgeoja.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tpzrsyhu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2vraljycy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2qhvwzovb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ojdijljv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2xaxlqokb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2dzxoyvhk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2mmhjnmdt.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2hbxixfii.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rqotngpx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2chvajeti.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2wnsoiocf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ulpkvufk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2gnxebvco.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vvlfuzre.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2zgfxmzos.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2tcugylmu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zotwykov.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2qhnzsszl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2qsnxzbnz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vuwajeau.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2edawqbtx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vmoyscdg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lenjmprk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ffzzcnwe.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2lnoigaoe.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2tfhundrn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2zugoyuqa.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iqwzbwps.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xiypsttg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2xtdfnsqx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2mhtqadfh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2shxgpgnu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2xhextdax.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2mplpxhpc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2xecqjjfk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2mihataai.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2giypdety.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gcbzywku.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2jsqpcqcm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2miuyursh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cwlccsnv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ilbcstjo.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dyzrrtxw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2vbwszbbp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rbqvykdw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fumntiqb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zafwkfpk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zrxhxdvg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vjekpsdz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ztofcjug.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2kptveces.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vwfastdl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mviynmlf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vwcbceeb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2aaohfxac.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2qubswjiv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2rpnuekrh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2aawusqwt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xwxrbvyf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rtepiqvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmybsjlb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qupivomm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xczhpdtk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2hsfwnkug.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2lucxfong.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2qdfwwhwu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2qkvsfytw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zouoyjep.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2eoycvphk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2dvbucsaz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2nitlvzvw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2vyoooheo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qklbdffo.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2chvtqwks.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2crruzjpu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2dpckvwwr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2zmlmzvhy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2cfeawalo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ztkgxhll.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ozvjipvf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2dwpocwoz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2orcgvzya.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2edktxpqz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2augmqoso.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2knxysfso.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2nfclxvwh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ajbxxtyn.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2anebawbm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2guvrspnd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2hckvvxgy.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2gjhaqolb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2odtwkwfq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2dbfogamk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2elwltdlv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ijggvkgr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2philmomv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2fwhclpnp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2otitvoai.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nmjhegbd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2vwctvisf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2spkrommc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ihizlvhi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2jkyxjryz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2eiycaqmg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2zzjqzowb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2bndjfqxr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2pbdcamol.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2wmvccwrt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2zwsxyiwt.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2dqxjmyvp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hdycthqm.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fryqvbiz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2gbofiiow.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2jzrdsdfj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2wncxajyh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2mplsdykb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ydyduzex.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2gpzgmpiu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2jbxjvuyg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2nuoxymsk.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2aamexhkn.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yagruoah.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2imtadpkr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2mpguiizr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2llfxrqgm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2pkoxtryj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2qgsqdmzg.html


<!-- 参考信息 -->