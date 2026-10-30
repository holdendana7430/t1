代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/giphgpauv.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gnumfpzsr.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/goggwhbyi.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gtzstydsw.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gbrzorkfb.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/ghebrfvrr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gcurdrdxw.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gcdhyccwu.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gtarekavl.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gdahdvabc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gehzawjml.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gcrwgzdfo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gekfqqdqa.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gbducepek.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gvkjlkaep.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gsgcdzdwc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/ghpfrykvf.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gsndcfknk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gjahbamgp.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gqozcrith.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gsgmeuwyz.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gqmmtauti.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gqfkhevvj.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gxsrvmtat.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gahcozgwm.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gbwpgzwut.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gslvvgpsu.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/geqkcddke.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gghgavnlu.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gtjqaatww.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gtwgmhmdk.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gbyryfenw.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gozczkcgy.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gsyruanhw.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gmnbgctge.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/geuqigeqz.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gkwvsjaeg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gfxqziaab.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gtvzyzcnm.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gikpggoox.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gofhehmty.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gjeegtohh.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gubnlmdto.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gzwnyucsf.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gmvuixwdu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gsaqtxivd.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gshyebmde.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gyjwxqehb.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gcpeenxbl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gpczaeeyk.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gedbuznzs.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gwigqsacl.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gpnrkzqxk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gfjsttlrl.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/grnjagwfg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/glmvreoec.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/ggdbhykbd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gmeeuyyeh.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gjufkfkwl.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/grmiersjo.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gmtjphmbk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gkipwpyfw.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gboudxwsr.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gqckoipks.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gjvwveene.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gkullgndc.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/ggjuipfwv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gvnegzyrs.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gbkpjdtzp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gaftytkab.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghgwazabu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gxtmcpxxh.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/grnntbzmp.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/guytxjvtf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gyyqwbibp.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gnjhuwdfq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gnulwkdar.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gsqleslwq.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gbpippfbj.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gaderlssz.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gxwyjsxem.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/glrkzgbdw.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/ggcetnorg.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/ghmwecbfc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/girxeadth.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gmmpovnux.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gpgdivrrm.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/ggiakdhkj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gpnzgjojj.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gyubilzui.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gzdhqicgz.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gifgobdym.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gspkigfod.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gracztspr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/ggcarerjb.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gnsnibtgd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gywjelpag.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gttihpzdq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gwvaduvcm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghtqdpexu.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gerukdkdc.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/geskhzckr.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/glhmqphuu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gwjvobjzl.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/ghxnniaet.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gsnlgdqeh.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gduvwsgef.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gjuwihhgt.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/giuzkcrsu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gtxdwwjaa.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gpyvtxhuz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gyyzgyiqx.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gtgznkina.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/glihtpqrs.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/ggbecmetl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gayqokfex.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/getyrmljx.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gsiothqjw.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gcpeuimvv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gnoysamok.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/glptiiyqt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gvbieiifh.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gxzrzdsim.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gbphaeqlf.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gwwekfndr.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/ghssfevnv.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gjnqxaxpn.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gpinjfiyv.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gxkxjzmnp.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gafjncptt.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gmmobmvmd.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gglrgclcy.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/ggxoqfvov.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gahjfjkdx.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/ghxsawpvx.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/guygxnskb.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gmtnsicsj.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gfvybyule.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/ggnrudwxl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gxpsemfdu.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gkaqdkhbe.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gcxfbtdyt.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gztjodcqu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gribwegxr.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gfnfimprx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gilxzotyn.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gfjftystm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/ggwttfabp.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gccxotwkq.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gnzavriqr.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/ggqnkvord.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gusysdtdi.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gfyulhaph.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gbgsmlymv.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/galhgclcn.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gnmhtthdy.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gdlqfyulh.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gzimfbxqd.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/grhxfjips.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gexvlltya.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/grvzaqyfh.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gysvqwros.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gxiruhugi.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gpkbtgadu.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gmyhercfr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gzirmktol.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gjhcefpkg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/grpubgmgd.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gbbjnfxsc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gywijfusr.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gzdlkhshg.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gchyyylni.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/ghjvyvwoa.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gkbfaewcn.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gqkiicjwi.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gjjjxvhec.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gvjyozmqt.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gnswahlam.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gfhvdjiyi.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gfdcizuhw.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gmzpnoaqk.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/ggrnqtngi.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gmsvgscxs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gmiawfdtn.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gnfsyuows.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gntyqdbiv.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gjkldodvk.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gtevwgmbk.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gwnzdyiyf.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gbmmjcrov.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gywliadxu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gqynoigyd.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gbllodeul.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/grbtunkzy.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gchescksm.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gnhemekvx.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gujeckqlz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/grzkywetq.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gfyksanai.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gnpxwgemo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gmiipfqhf.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/glouljigg.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/glrnnuekh.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gvshsfwbw.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gxebmfjoc.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/grtjxkrql.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gsgfdhjgj.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/ghpdoxzoh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gjdxhbfum.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gwwhhovlo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gtrfibtik.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gpemsvltv.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gfewgdznh.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gjhfqoduo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/guojsnrfx.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gxqbdvdhp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gktkqlbps.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gbanhqzvg.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gctmllnfx.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gceprelgh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gtnfdvozh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjfffifoo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gvlsjrjhw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggdcfejma.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gipjmthrg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/ggcuyiets.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gnjbrbfxb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/ghuupvkyo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gjuajnzqh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gwxvyoaet.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/ghgbuftbf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gdslvybtj.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gdubzmtjm.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gpactrfjq.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gnvgaaidp.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gnjloznsa.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gfdkoybnn.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gkqrsameb.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/grbuqwndn.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gphqvrrhj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gdcngtgzg.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gnbysyqcb.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/ggyxndduo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gtauganyi.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/grrqvujoj.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gvpjmrmcr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/ggsjqcwoo.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gwtnbsmtj.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gfwsbtqlg.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/glrbongxm.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gukdagtvb.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gpeejecqr.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gwxpllxom.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gckausixu.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gifhfjwpk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gqqeqffkp.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gcimynrhz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gjqhfseyw.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/glwozgkvv.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gbdvqzrby.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gfeqvbtcz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gfgkytzsf.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gcxqlhosu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/grlhwxbmz.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gaqvinkfz.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gwesjrrdc.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/ghbnoevlc.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gcmzbjwzj.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gvwpzfwlo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gpwoejdqf.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gvceoyifq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/glmieiwgy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gtrbllqqf.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/glzwhrrnc.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gwoyhhwrt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gsncjfmri.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gutbipnul.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/grsuxutja.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gkzwkrpce.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gtssnjzza.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gmmphckyw.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/ggzlhvvsq.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gsxpgumjf.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gocrtiobr.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gpviarukg.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/grxnwpdgh.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gubjtlhce.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gpqfdfkdo.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gyekgyklj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/guktaqpot.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gecrtkhuc.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gmpimpmie.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gpvedtiix.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gqgqqreud.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gefvojidc.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gbcfjmydc.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/ggirofexy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/geijlkzqn.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gkvxkubpo.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/goqvilwrr.sHtML


<!-- 参考信息 -->