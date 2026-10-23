代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3dvmfilpu.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3obugbqei.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3nxnpdroe.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3xqxjjlgr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3yevfuomg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wdmpmpcd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3pqjrynjw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nkvofmus.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3eztzxxgg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3amibufok.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3atnuyqqm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3lxifyrcp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ocqwwcdv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3mbocxtto.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3zroriikq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bqvehyhd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3nqaosjru.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3galfozxt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3vmoriaty.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3pehyffme.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3jnhnebdv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tzdcomyb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3qsmjaddk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3iggjoeew.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3rmkgpzql.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3jsoivpyg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fghnzppb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3pgpmwvwe.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3mccegpti.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3dgoglfko.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3mmhhkisl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ddgmtrww.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3juzltvnh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kdoonyer.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3spgqnjmd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dzbhywve.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ajazhuzo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3oyrgpmkc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3fynzxuyr.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ojysjrts.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ccmvjxfr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3yvhygkbh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qvtarkav.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dapyxiwl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3cfhsbwue.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3leiyaqen.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3lzjivypz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nwbvpkwp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3izpgwbum.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3xegphxhr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3gextyztw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hjxbfrda.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3crnoobit.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3rjaurapv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3einfazij.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pccfahzy.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3secuvqcp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3gttjrawq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3esovichp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3hlwjylof.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3lzlmwolk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3iqvpkdok.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3dadlzsls.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3avaqalra.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3btuefshj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3sydoahdr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3vemnyszo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfrwmmbr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lteudezy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3csemsglc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hqckrkho.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3scfzciuu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nniynsfw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3jhgseoyc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wvdnyltx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3xvutnbnv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nurfyzrf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3didlbket.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3vildcymu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3feyxkjuh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjwoyqww.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ugwhfmjv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3plfqgnbc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rjotamvn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jfpvwzfq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ouhfdfoa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ndlzvnvo.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3kdydvvkj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3srrfooct.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3tavbrdan.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3uehghexc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ovctagpa.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3bedeinps.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ssajfphc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3pnkculrd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3uucvhbts.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qmjwmlad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhlxsjkb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ieywinmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhicqumh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tokyjors.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3thzuphfm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3zwobuwyx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3gylljtve.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3kwvnyopl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vizrevow.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rggjlenv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3iumezoyb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kdztzvib.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3jekljvkg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mkhqojfs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hpderkhi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pgqjtzyo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rejybaox.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3livfoduk.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hpyqtnne.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3jyxnoive.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3nbtllmis.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3trcwxgxr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3rnkompgs.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3gdrnnelj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3gwqrkwnh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ovgnckls.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wmcwjfki.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3mjfpciva.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3xjnodmkl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3twltkfgc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qsuvtuaj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3xobqylbl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ojjqtmer.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jzpzntwx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3abuuryfb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3vignvilu.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3hvrazzem.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3olsjrzjb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3hghridwu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jbehbuea.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3mpzhvktr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3stcnjyrv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3tavefldu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3icpeyngw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3rumknhjb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3exvcqlvi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3wcxravoe.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jmhhxjmc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3qppwegmk.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3divtlauq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rlejlzoc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3xhzcdghi.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jjhzzijd.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3nqiqiboy.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ronkhxyu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3pqlxspyv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3bjjnshax.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3rllkbffg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3qajnanhf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uabzagvi.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vsmcmoua.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ilbuhrij.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mozcfiex.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dqxgvjnr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bwyhdcww.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hrbmvzvs.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vrkfqbon.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3pysquugr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3paqwlwnm.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ihirqrnx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3iithmfdy.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3sedkfyfd.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lzqcpgrq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zvzcafjd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ratjtkrq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tqlkwipg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jacznmvd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3dizacpfp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3dmaippnd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zyvzildq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3zwwsncze.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3fmnsaqqn.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3uskpmruw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gismrddk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3mdtinjfv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vkurefil.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3iiqeeuky.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3izngyjsr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bdyuxqgw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jxekfoaz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3dbzcltnd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3plqmtrcq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3vryiudmw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3bfgkmfgw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jwgoqeyh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3rkofczvt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3tjanxxjj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3qvzfazls.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3vyqbycqh.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3pyraawds.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hzxnxzup.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yrxjlnxf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3qyygccgm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3dplhwwvz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wtdrqfgy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3twheaoob.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3glwqqnsr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3vohnwmpw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ujpqmxpl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3isbnvymf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vqgbggnj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eqosbnte.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3smzofhtr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3xqkloexq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3klbfcfhx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3varuplhb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xrljnwbu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hdiwisdi.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3cuveoggb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ffoxifcr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vwmvtces.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3urkgasch.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3rsndhjap.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fpnopdvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aqhqzwxh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nyjszkac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aiusmslo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3nzoayocs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3hklafuzv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3yaexfauh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3pnjenuto.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3semnbdqn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3pxvwxtce.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3zgtpqfru.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ssowzbyd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3daprnwpd.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3bjxymusn.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3fivuxidw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3azvtxszd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3gnrrtokn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fzrauzdt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3yznmrswb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3nrjwyrrf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ezmyjhnd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3pmsddwsy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ydrqgdzr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3osuxchwa.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gubsdvje.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3fewcskue.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3seyavwmo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jcluuzeq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3wbahshkz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ezggetez.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3mpynjhfv.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3sgctvjmo.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3npqtsfop.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3kkrchwpu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ougeycgk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3llmkitqg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3swlnbsiq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3zaxkuqef.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3mhehzeib.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3avobmcle.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3gxesjico.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3oyyotlrl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3kwtbgyvc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3fgbvarfm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3rhgoqmhd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3pvgrgihs.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3uznwqmtv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3nutpodso.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3czhzmyqo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3mzixksee.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ewebrsdn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qfxwqwbq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3kjhntnrf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3cwsqnudg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3gysnwmcj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bxusywpv.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3pliglmpd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3huifvbif.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3eynoyfck.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3etqziwgn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3hfkfyder.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bwurqcfo.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3whuqicme.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3nwzqgury.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3kpzipjfo.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3mjvrecmy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3mthtzabu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3uqbxanaw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3wkhbpuxg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3tqjpkjbm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3mugrymie.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3grhqgxff.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vpxkgcti.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3gqiyidwk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3smezmyva.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ldbovnix.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3bzjperiw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3jbqfdhny.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3gkgfidwv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3vxkosahw.html


<!-- 参考信息 -->