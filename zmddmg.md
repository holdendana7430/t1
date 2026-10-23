代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3udzdczta.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3waldbjix.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3jihgagjq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ulrrsoel.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3rtsuypci.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vaigbqfz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fvhjkwcu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hdkibfzi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3apbqtbxk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3yscfkrfv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3zrhtupsg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hlipzjhi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3tqrlnclv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qdgdccqo.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3shamwtpi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3eeluvqje.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3pmlpbbro.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zybmnaja.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3xweuwmaw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3hhqyysuu.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ifsjvwmd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3egsuxqlu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qpflrzjs.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3fxqoxnkv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zmyjnmnc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3enljahsh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3jweaqiyq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3tgmjccsd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3xomndwpc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fuljduww.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3raqaxyow.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3lywmstkr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ahdzllyn.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3psykdadz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3bteojxqr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3gfybauws.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ywnmsjqt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3jwrrjmdw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nxljhohh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zizcqhta.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3jvjezqse.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ackyleds.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3kmjpvrre.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3jzxziaqd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ehxpaqnf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3jgwntbod.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3trxxcftm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rldnkztz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3eemptuth.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3topjhfzz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ustimzul.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3snkwqojx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3hlkwerek.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3bkyuiqhr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ntrbgyjc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nothivcj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3qkvcxnwh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fmwrnlbj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3sfezwlbd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hermfxqf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hcnjbddh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3bvpeqpqk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ynbhyuye.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bzxywvdh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3hhhytcll.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wwfeouas.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3dvcyznxu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3bdqzgoha.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kwsbnger.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3bdkfkjun.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3bbekspwt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3toxkybrr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ilgfqhoc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bhbbvwbt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3giottmkv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3puumhjjm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3yxghhple.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3cajsxwos.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3cyomjbqf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3difrvqge.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fverocmm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3crtlvvtu.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jastzgub.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3oolbannw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3pqxsvvaf.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxbrflgt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3pyprskap.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3hjyuxtmy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ezxwhwls.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3bwqdblnr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xnxywaui.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3tlbxwtvd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbdulinf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3tvwglbsh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3gpokyize.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3qfphkdbj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3gfechcrr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3lznracki.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rfqywjnq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3fdisuonh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwjetfdp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3dufyqqln.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qerhuzpd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fwoomwfy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3xlpgsdzd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3fuuzfrco.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3dviarleq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3gidyjlxg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3kkctclur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfcekubg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jzvcmtdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrbjvclb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qcbaxuxy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wtpyslkx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3zumhmfeh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3lnzibgsp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3sazoljdj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vcsacdbj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rlagbnlv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3alolaalr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3yjhmvoav.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ljoivsef.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vrxiecgf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yyhkpdgg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3naajmyec.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bmgslmug.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3inbscdlb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3axsadkii.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3chfhlczm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3odsjczcb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ijiybjxw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3kztgepcp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3idpchynp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3vgfqhxjk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3eetotyxw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bhkqgyvr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wktpkvrn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pztjfbvy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3prgdzbon.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ghnyzvnl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zujleloa.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hibitkej.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rmoelqiq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lhvhsipv.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xvmhbsep.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3gzrbzlte.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3astugnvd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3nulwduwg.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3enfghdjq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dbgypkpe.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3nlexgcel.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3dajakbxu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ixpmfapz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3hpxmwrgk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3hsfyktvq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xwpsunlk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cpeuhmjh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3mvyflomd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pxydaclx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3enosfcgw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3wkzbfool.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3jvfkgkyz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3dxuubriu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3xubpwufg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3srfozwgu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3bukkvzsc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wlpbswso.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3tripsvhs.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3fdqvepia.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3loxocugl.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zrejumny.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3zevxgmay.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xkzntbhu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bajpuwbg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3rltmtjan.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qchtfuol.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yvlnwpvp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3kuglhwvv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3gabykxag.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3vnqxosrm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3nhpqjxeq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3uydywkse.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bylvqjql.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3rjgntlpx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ktiapdle.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3mvjywxuo.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3knfpkzgn.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jwyzdvum.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tmcvgtkt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rqqptqvq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mpbozhon.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3qigurzam.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wolsddqx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wxpzsvyn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3azaavleq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3krioubyv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eymyrggj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3cahzqeuw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ticbkiby.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aekytjey.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3beapxpqt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yaalvszw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3nkhdlhlr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3wmtceukw.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3nvptdqhz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3tugmqwju.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3bcbzrqhk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ozwfwdnf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3szyvxwlv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rablseip.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hwbjfpjy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wipvhhns.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3muqstrkk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dnelrsbq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gcqisffj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3peeqjlvk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3pxtaqsjl.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rokvdocr.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ktgcxoyf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3yrxidwku.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3sbttgzmg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3axjyukha.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jjrmakro.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3schymcse.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ueorttvt.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zkkhgfri.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qpfrdoju.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3mngeiynh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hrdpwqff.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3wytseato.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3slbsfhrl.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3fdjamrcu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ehascise.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixwmeqyw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uulewhjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epntpxxg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3vtxcysex.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3rngylfdv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ktajoldy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ixvyvujv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ztbyfhvi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3rgpdoqbc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ioponhlv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3uqffnkqw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3vwnhguqa.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dxdopoxm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3jqpuilau.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3growgxhi.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3rbfjkuiu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3yszlpwgu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3duxnkzov.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3quksnhbp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3mgcbgvwp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ptelhnhg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3wjhgyoqq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3imfsrrjh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wzouwobo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3kglpndnu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3uobrbmml.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ejjesfrs.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3azcmprvy.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3qugswxcf.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3uandxzkj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3laiexagh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3umfyonuu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3dclgtdoq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3notbtkps.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3gkvgtxnm.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3uujqcbvc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3zmtltnqq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3krerhvwn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vansppvw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3fjwkpgbw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3bapqhquq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3fwhtfhei.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3glhnwwoq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3owiietzq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3wixrqcoe.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3gpljiqaq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ihpdmvqk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3oozlbizu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3daekolup.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3hluimevg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ugekjgmq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ygjbtozf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3iacysalf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nilackeh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3mmlniedq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3hytgcocv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3mdqoevqz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3fuiznwak.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3xbojpfqa.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3qfhahnjk.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3qvmhzspo.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3tqwcfczp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vpnmeccm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3qjvvzuxf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3hhwvvvzy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3nmfshydh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3vlzyrces.html


<!-- 参考信息 -->