代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghplqabwx.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gomvukbfo.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gysmqykug.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gwwksqyhx.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsgvprat.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gxmizyvmy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gzhhsibqn.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijpfhsnb.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdjfoebd.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gnzepeldn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxwzqyvv.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxrddzie.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gurtvtzsy.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gjoddwngu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gssadekqo.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/geiixczyx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbfrqaka.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxcgvpby.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrxxounx.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrrbypqv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdadowshu.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/glupsowis.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpeefiid.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gfabsfdgg.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/ghnhnnmmb.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/golizcmtg.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gggeoexea.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmdigbvol.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gcogbbicj.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmsnbjah.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfosxgumf.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gpfsbnfkp.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiehzwvt.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubautwck.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/geqfnuysw.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gklvoycsg.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdftsdgs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdgpedesy.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gapvnjedt.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/ghoxcpawm.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwtlybvw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqbfjqri.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukxvuwmm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwltgtgcr.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gjvrrmfok.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gfgbhuprd.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gsemhkbkf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpekmtnks.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gdsnekkfj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gayggfnve.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlqkjfke.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gtkqkkotl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzexpiups.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjcxixwr.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbinpoou.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvatvdvf.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuacrxnr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkgxicgd.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gjbwpvxxc.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzdyhipw.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlbhqfhu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsthjvhfj.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/guzjoywjk.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glflmphkf.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gxraafrhy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gncavlxzp.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gtihhkgzx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gginkjfmr.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/grcpywqcr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gthbxejtc.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjujjukec.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gojnwytzv.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfoiioqq.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvemaspzy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecshsshl.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxedckwx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/grypnpwxr.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gktcwqslx.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/guenwfzss.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gmluzefdl.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gieuvfvsv.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/geeykngtp.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmifnxgi.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gudnddnum.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/genauxwof.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gfydvyqvt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gskiyqkmf.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gphacrqvm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbqdrafh.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevhhghww.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gnchitbgt.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gjorxyuii.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkzebzgh.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/grkidkagh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpgkmsah.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjnpczlb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtplwvtoj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwvagblk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gphnobpsl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwmzfnunu.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddmmioqj.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gfmyplslz.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gatmxwkfy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqfdbule.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpzmyvkt.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/giyxhafet.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gxcnzfosa.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gpehbkfdp.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/goxtktydw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpcerfsc.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gkniuziqs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gooygympv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajmlfkwl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtlbilfv.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/ghepqvgvk.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gezwwswyy.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gyqerauoq.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnfukzkc.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczoxxcce.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gjspgnaww.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/glfbumzjl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqwioyed.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gylbpjpbb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgmeawwq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwywrbug.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/glgfrivup.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzhvuclx.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gszbjlnes.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfdvuknr.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfbyijrt.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoxinqbc.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsiozbcj.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhpgsmhn.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/genlhsnxf.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqwgklmh.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvienidpf.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gknfhcssg.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaonrsue.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgsdfbcf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxddyvsek.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gephfmzzy.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/geqjojnvh.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgxqzdze.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbihsffdy.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgjvqrho.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gevgtrjck.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdnfrgci.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/grufkvxfp.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gbvmmjjmk.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/glfbresaj.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gqypfozrh.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gliygcnqg.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/grudoixdx.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gnmqvdbaw.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/ghhoyuxyy.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gvscnunag.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/ggcvzdnoj.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gfdzsguie.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcshhqas.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkvytfoh.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gwddccgie.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gtkdgddlq.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gmqguwinz.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gqaxrbgki.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfksmtjvo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbyagqdc.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gihmjjlso.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gfqwfrlcu.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvplgfoa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruamywyi.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzuvgbic.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/glzgjzrqo.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gnbjthdzz.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/guivxduop.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbalpdmnx.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gmicwsbyx.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gukdmkqwc.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmymgnvik.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/goenxolqj.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqtvoipl.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gdpygoodf.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gbafwlipz.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gehofrdsy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gnlrpmomj.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/girigqptj.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/glglxhslh.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxwauzak.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gedcpezay.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gwxsjzozf.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gogsqctmx.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/grijlpitz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gugazxvnt.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gihwoqpvb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbgwaogg.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzobzcfj.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gnpnyvfjx.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjvseoue.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgnpgcye.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ginvglydk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gyoahcejw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/grcfhbajq.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/grcjeqech.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrhjhrrb.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtkjefysp.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaprzwud.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfikvzmv.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/ggmhblagg.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gqptnynov.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxyohutg.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gewqdbfnt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbafbyuee.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/glkuzighh.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gsdulusmx.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwforzvkc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gpjegwsdy.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gcndianiw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gnrvrowsj.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/ghrikjevr.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gujnmawnm.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gibaavuoo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gykxeiqnv.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwfyzwsaz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gjurtvrfr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gybkjrqte.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfwvyggs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgjwdmeq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gimjkmzef.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjnttdgvf.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/ghjfvwuek.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gcmrsywql.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfklusyv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/girdoidnp.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/ghuhwlgtp.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gwexocyic.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkztvetg.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/ghgwxrpxj.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxtgevqx.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpkotcbj.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpozthfh.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/glosohozk.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gfjpwfnyb.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/geuqehfxj.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsshhuyy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gkmyoxzuw.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gczxgxjoy.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gmyvajwwf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gswqctpdg.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggshbkiue.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gqkzcefdt.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvgutony.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gusxzhcju.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqscmwxn.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gqcwhccml.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntmrfpbk.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqdzmvjy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gnfmesxtt.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/glxgyocka.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdorjgaaw.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimuxqxyl.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzucfpwr.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrozgvch.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxxohxmx.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/glqchzfjq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gmmqxdecs.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjlobnwr.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gycgyqppb.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxxoxpqf.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmuhfper.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxskuyze.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gtviplawk.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyhigtev.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgupzrrr.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfuxcuss.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gykvxxrnq.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gwjifwnmq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnerixrbu.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gudenwmkg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/grhujhrjn.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gryyorbaz.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgsuiwbs.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gkflzgxgd.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gqwwwmtii.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/guvqkzkri.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gtoatstkq.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gokxiardx.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gnnnkpsij.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gboaxggef.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gporyyspz.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddprckwg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gypoywuad.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnrcusdn.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gzicvqzaw.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrxfcnni.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwnzpoth.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ggimupvnc.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gzbjygsdz.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gemengttu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnekifdv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypgfxgke.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gmopvpbij.sHtML


<!-- 参考信息 -->