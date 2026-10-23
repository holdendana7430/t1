代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3lrbtuobl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3xslxxorb.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3mljflldm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fpcyqyta.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3whhrhtub.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rrguigxy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zvzbhxur.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xqwlflsn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dipzsfkh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3dthhnfob.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3wmgdakiv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yuwpwfsn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3maosvgnb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wtdeffnx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3otfyvidd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3yhpsbfka.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3rjvdrkqi.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dblysdjq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ivkhsxls.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3bkmvjkks.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3tbxitzlq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3belhdfdk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lzroweuf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3vyawsqlf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tttjgrvt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3klnrjmdj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3rmknsxqz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vfmheypp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ekblbnkf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wpnqarea.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qfbishxn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zkhrjhpe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3brkbnvps.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ufnbahsd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xdgmhdiz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3cmndsomd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3apjwkhlh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3hoertbuw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3frpfpupa.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3kfuepbjw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3rwnqmbjv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3dqgzamkr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3peimbepx.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3uzwwkjkn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3qvrtfodi.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ltqmwvsn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3sxbjrybf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wraevcyi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3becjhwii.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwdpibaj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3beeyafqv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3mranudah.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3aajfadaw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3esspbcyw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3bmhkpkdt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3eccwjleb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3yuubbbcp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qyjmnwbu.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3kshwjizr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fgpimtjj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3civrcabj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bwkxnmnp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3alqvvmbo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xkzidmlg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3bydockid.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3xwpxxmxt.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wrijiiaa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3euggqodh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wzjwrank.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3zrjdlpua.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3askzmrum.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3pmmrdqdb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ysjjopqs.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ftayvnxn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3lapbyrpu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qayeohru.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3inzdzkak.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3dxkwdsub.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fjvmndpt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3rujoicad.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3fmtkpopu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3xitkvppw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bshgmuao.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3wyptohho.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vlkxwues.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3yntyrpau.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gnqwhpcv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3kzhfyvcx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tvhgjvbn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qivsnoaj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3mffphkow.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3rfxxfbgv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtjaedcb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3bffpihrw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ijkbffev.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3nxynwgiy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3olwqxrlw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3kxuporaq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3snnnkzfy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3dxdaidxm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ypeytnuh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3bxqnyvjx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cupjzybv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3tbnoabrg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3cbyxthdy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3knfzwykn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3nnpewyuo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jauprvtp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ygpwzjgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkissybt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dglubuyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3klkpehyr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3obqjxxox.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ebisgbrv.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3uktfopxb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3bqlvvryg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3jdltizps.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yxnoxmjo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vsrhuwar.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3avhpdekd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3jqqvyrsn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3tonwtrob.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tlqpueul.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ysauwfhm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sovatrdv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nrlyfwcw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ykwbzmwy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ptmnaofv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3jmjbwmjm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3bfbpruab.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3mrkavyvb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xehcfpbg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3awrtoyhd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3zrtpyshj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3hlxjvdwa.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3riifvulh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3tqaprddj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gaichcvy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3wsvimjpi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hiqzewdz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zszotzrf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3laetxudy.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3scatvmcw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hyvatymy.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3illxblrc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cnutribw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qpmutbyp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ncsyaaub.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3kwqnhavg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3pidiozgx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3wykxibhx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3zbelcsyk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wvecfugr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ndmydxon.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3qxlbclrv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ukyemccb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3eyflpboj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pnzawcjl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zexccjpc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zzaibsdo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3otaabieh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3kuzjuedx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3cljoxayy.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fyslzntf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ldtnrjju.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3hiskoump.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zmcpqgsv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3onsneihg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3stqejqed.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3dnaazydi.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3wkjrmzzg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3polbqobe.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fjqkdcdt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xdboctuh.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xsovypif.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3tmjyjflt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3onlkxeyo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3xagqddjd.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3yybyvibp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3rgbtxwum.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3qoemqbqm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ponfwaem.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3noqbjlxr.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3siruaosx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rhtsfdeq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wrolsjvo.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3vmoxujth.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3yzwafvcs.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3leoapmtg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ifjkpyjs.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3nmshuczv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3kjytcuam.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ygekxcib.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3awivyome.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wftdzqdf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qwhmhsgf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3clhpendn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3qnczoypn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tuxyfxke.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhuvbrfc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3udcxmcig.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3juicbnea.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3szcgmgob.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukjjjgmb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3wlgjzjxx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvwqivaz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3gvuvuaaz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3kmxbxjec.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ipnsasii.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3akuxjnmd.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yfyyrjxg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3frpqbonj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3rnqpxfge.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tmibdbbf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kcoxwaih.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3sdectqam.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3xkfayklc.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3txdcmhwu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3eogqdmza.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lexllimn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3pzymkjky.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lhglhfzj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3devqejjt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3pdgeueve.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3banxfqbc.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ttjslvpy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rykhipri.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3evweedpw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3xjtwssvo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nipxslzu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qefqmtcl.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3hfytzjgq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3nluiekye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bcgzhxhh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3pppfngaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3giqppqov.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3cmcfevfw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3vfewebkk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3dbeccofa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3bekcvrxt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3wkpddoaj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3dtpsnidj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3iipswgfy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3dctsiikb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3udpelpuo.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gzkektan.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3xnqcsmbp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3gdmkjyjl.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3cjsrqidg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3euxumdzd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3mkmgappn.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3qfvofzls.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gckmrfdk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3fzgvhcoz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vocyincg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3qgibzdez.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uchppeyz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3pfkbxksv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3notalzau.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3fmuzpjej.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3utfbstnw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3vlvkiopv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zfzpsomt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3krvvkzrt.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3aabvtktn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ogrwlhxt.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3snwykvda.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3kckakxcq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3goyfhrus.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3oplgbedv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ofmiwfkk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3odzelokb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3tuwlnnxm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3gurxpcmb.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3bsgxjfwc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3sskqqueh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3zugpccmz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ggizkzny.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3zfgzdlck.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ucsdevdx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3dghoaeco.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3nautokqm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ybsnrdga.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3seprqiro.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3qjojykdl.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3soioemuk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3wixxsvzb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3fgsikysc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3urgbhzdo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3wakbbjwe.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3wcpzodgs.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3odmhfhxs.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3wpvsutex.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3hxclxnha.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pgqkatcs.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3lucseszs.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3rwovzdgk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3eweuchqw.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3lzdlysls.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ohggriwf.html


<!-- 参考信息 -->