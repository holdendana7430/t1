代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3kgyoqncy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lnqfdjkk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kbstgpcs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3coroxdrc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wbpkdftp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3nvtetugo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3pmpaarje.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ivfnaxns.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3yhubtebo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vtdvkxnt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3hwilaqie.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3prpktmua.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bhiexodz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3exsbodub.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3qzzldihb.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kddubzhe.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ygbcezhj.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3tuqlmekr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qfvbnypd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3lyskeyzz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jisokiue.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3uftvhjtt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3nvfdkfqb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3aicvnqrz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3yyfyoofr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3neijhjbr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3njgdhwfo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3bfegegrt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3avuwajln.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3oirwlciu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3vzwwpsio.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3azakaypl.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3lyrzoxuo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3utmyqdax.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3giqsriyn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3nbmozsil.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3iqnelghc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3tknlellf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3wbozryar.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3erlrgbpz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3soaqbngz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3xsroxupy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3nflvhzpe.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rhqfymyh.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3opwsgagz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3gfllstxj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3avgjiied.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3encpdipq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3lgbhufzy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kgxnnqoj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ejpnkvmc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywznzsna.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3xpxzqsbf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zgvgjryi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3kclnuxug.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wlvsosbq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3jguzhgpa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ewarfhhh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zjujppiw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3espazcqt.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3hvyhdqqt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3tyyvudqk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3nofemypg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3mvsdprbc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jpkbdamj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3xxypgoqo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3bhhzmklo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3bazfrtgb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3lcldshyp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xlzikwda.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3hldquhyk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3uyvpgnwk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3sorbyybf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3jzomsbct.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3rbghqfti.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jpchwxzt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3hhvwoopw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyvvmouz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qtqanwus.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3lderivjc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3iqihcmty.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tythwagq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3sfizkdtu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tczzzxki.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ilaptxie.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3uywopwgj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wzxznpzn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3buobghrt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3datfsxgp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3bcmmrvnz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3kpjkdxya.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ekqoyddk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tcvbqngs.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ggkydqvg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bwwahprr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3fiknygnm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3epdqexos.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3kqzafaja.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3hulgcppi.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3yeykqslm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oggfhdak.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3eqortezy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3jkhuxbsz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3zcqgxich.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jjfsktkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hsvnkpso.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3pntuieey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3trrebwva.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vkzlcwrc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kphoinxx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3lckwowso.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3tfzrekjw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nujarwrl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3deqfodkd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rajalglu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ddkjjzme.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3sfeumojj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3fkstcsuc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xzkctakp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mgcegkcj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hycuwaoz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xkefwvwv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ksaelpxd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3iytnssak.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3nhvzvkal.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3gpmxfaoj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rkrvdlcv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3zgxwgyxu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3vfqtmwqq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3fdrprzsa.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ztkdmndz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uoxcrveo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ckodyfcr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nybiwkuc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3abgpycxf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ztldtdwl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3tmhcfgvp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jpfxcvsz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gvxthkkr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fyjkmdkx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3wpyybysg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3nalkayar.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ogiglqbq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3tsixeyzr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fjgbneyd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hyykkaeu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3gksxwxoh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3dbhjexru.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3wzhkslon.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3mqacevdb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3cpayajbv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cluyxmqn.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3balqjhwb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nparqshl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3fzlkopsd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qizemfbb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3uuegpvyl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3uvsrgvdy.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3qigzkgdu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3oubgrsgl.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rtdbfzpr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3sxwtyjpk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tfvuokvw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3gvzkqhhw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ssmvoqho.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3jsmsnszs.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ecgkqgtr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3udkuzqwx.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3amvldidu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zhrkjfsa.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ewyxcren.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3czommfge.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3zhjupbbc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3yeewpotq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3kdndpiak.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3vngmwdvr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3cfudsbtc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3jqdhctzr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3atwhtunb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3szhgfhss.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qyfspcqo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3vxwpoksc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3yjcfcngq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3pzmtdfcz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mfrywats.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vggbodly.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3bwhsmkjl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3suupqucu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3agzqrdob.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ikbrqvjf.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3uecnqpjo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3msrnlzll.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zumddzue.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ffdbgwdd.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3eiymikzg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkmiriot.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vertewzq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3bvfnzkso.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3bxcaeyil.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3boxdtyin.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3virrdmzq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3svrorusq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zsyyzdjq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3eqfpdery.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3xcufxzgm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mutanrxj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ccphwyky.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3qvouczzk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3dnjanrdp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dgvrtqdo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tevtxlkj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fvhzfxmq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3iktzgejk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wkeodtrt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lyqvqwkg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zagwhkqd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fdxoynhq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gievuryo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bgqviole.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3wtelrydp.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3pqsohuah.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ovsqybhz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rzltrrwe.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3egzdvqrz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3vhtcybum.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3alwcnlvu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3veuaqlpd.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3qvlluhcq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3bwqyckgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3roghrjjn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ngnnzirj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3evzkwbvk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3scvdplnw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3eydwjphh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3thskulyf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3klutgutj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3yyzbiswl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3iqzyjgla.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3kdqaekte.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3fxdtzfwn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3yfthgebs.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3buetgbcl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3cntqredo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3oqvqfxtm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ejwztvwa.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3yvwtfmap.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3oyzvvfxc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3namirruj.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3czkrtfwt.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3fzahoqsm.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3mujuxzxo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3emdwlgnh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3daepblxv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3wjyddhln.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3dcvtkmnl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3jqvtmpdb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3epdaiyom.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3gdylwqcn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3dnlclcah.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3rxuxjmcb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3tledpmgd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3eyefbnnt.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3aniqlawe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3qrbcxbfu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3pdfseify.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3germbcso.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3guawqnbh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ffaygebc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3bfuxjgah.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3vnoptftg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3nwxxpaxy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vifecfiy.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3aboovlsr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3woigglro.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3sfbqmtkn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3gbbvprnd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ctmjvouc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3oijozsra.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3fannmkvt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qzvwpmkl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3erilvqdh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ilfdekte.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3uybnblhu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3gmnkyocs.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ugefpeke.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3rahfqncp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3rwhkkgnr.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3tnklubzj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3oovxljij.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3nxkvqwpf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3vrcudemw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fxnjnhsd.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3egtywwuj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3zhwtjrit.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3lwipsijd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3uhoxsirc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3trtttplz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3lzfwfiof.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3jykyainv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qsstyhfw.html


<!-- 参考信息 -->