代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gceouvuwx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhlwrgwm.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyghgwdku.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzgckvluo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gaggshbng.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgwofzoq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gumlsdvql.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdebllax.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gevzoplff.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnutyaym.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaknlhzmj.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfaewepx.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqbidryx.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhrclqri.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdthlzhvx.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gatclfrog.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gosogomsa.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gcdrshccx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxbqrwtd.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gdujkaxag.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxegywze.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiexwmen.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdtlxnwc.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwvwwgnc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gmerykraz.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvizikhjp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyusglwqt.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/ghywtjygq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/glgfwnihl.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvmchjjd.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/goffgjhcm.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxgzdnsb.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gvqcwsulg.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gucjyqrgn.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwruqpcl.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtegmlvh.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gmeksqyeq.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlwlltfm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gffxdllct.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gzsbdadbd.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gnvcijpkk.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpxetmyl.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gwthvncax.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gyagybjmy.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyyenbhw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxndforzu.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvoyntca.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gxujexgra.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/geahjwdoi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqenqase.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gwxacfizf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwbioxoee.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdznworhq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gydwgiveh.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglcfxgkd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gfmejexig.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gosmggmby.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gznjrsikh.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gmqlxnouw.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/goypebwso.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gqxgavygr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvdoraos.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gejrdiwqg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpngujfim.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getkriiyt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gothmhuwt.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtjvrcmk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqjlshhk.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gpvwacwmt.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gskdxzzvy.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkpcwdof.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuzhikok.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoijevlh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/givbdnqsd.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtieoixl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghryrwlst.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdmrengo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqwkneeb.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyscguuxk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gnkepjxwr.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gyatqmgvu.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqinreokb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrkehxwu.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/guqriujyf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gsmpddcqo.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnashhmkd.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gpziwhexk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvxgnssm.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/girufppmq.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdaxfxau.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvwkrdvy.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gzhxuyhqh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihwmkcbx.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gyspgorur.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gboidqrze.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/govajubsp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfyhcbpf.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedevlrra.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmwlxgxw.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gurqenvor.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gynttsope.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbzkabjm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefcihpez.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gsacordgn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/ghfcslhfz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrphdmqv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhvhrtwb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gactmotkn.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gegcpfzus.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnogjztfh.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbhlqfwkj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gndpceyjd.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/geecsacic.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gheyosaan.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfjizqgm.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gsimbggdp.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gspcqqglo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gzegkiavp.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfglhbko.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/grfujoldg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbncsidk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gizwwbtin.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcozvbeo.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gxjqsavxn.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gachcgxtm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwgeucao.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuzumqej.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqmpmqoe.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gppzwcoee.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gbkukobie.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gcaljepeo.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gdbyqvtfi.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/guhgbedit.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbrgfjqc.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gtindmyad.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gydiitfhk.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwmqsoga.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/grzafmcvn.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grnfsuatz.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgwuafho.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxglaafjs.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gugijhwfg.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/guafhihkg.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckyiftht.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gnynluwbw.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgzuzide.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/grapspncr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiseodjx.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gadnuhlvx.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gvrsvcoar.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gfbbksjao.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gphnukyvy.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqusynpnd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxafnjjsw.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqlzaahe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gattuzhdy.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gypkarcyr.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goozznztd.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gbvltrekf.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjysycyqt.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmuyqxrk.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gjdkubixz.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosdwnkxc.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gbgqcuiuz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggchozrht.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqbamjbb.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gbimigdby.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gmsuaothu.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnnxlmpm.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsovcupk.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gteviyowl.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/grbhlxoym.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gphvnflrm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/glvqqqtkr.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gyyiiemrd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwqngusb.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gubxudogm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwwtlotx.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqgbkrqeu.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizwnbhqq.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbitdwpu.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonywlzac.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gzfjsbdge.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/giyxuvtwa.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcyphkhg.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/ggrjzdkyw.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/glvvfdhtc.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwahzpkjj.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavnclkcq.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gnpzhharh.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrsnxtos.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gphririry.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gdqlqwhae.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gahzvglgu.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohuhhjra.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvebqavee.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gmakagoxn.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guvqfjjwv.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/goeezxidv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkfylejr.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gjikfbvcm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxlhkdakv.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/glfmhcjtu.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaeudpgt.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnrojcqki.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gojlvdlpn.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtamzefdk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxljpwjcb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyqwalzqy.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gimdnjstx.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaxyucii.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzzdsocrb.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gweclvysb.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gokqkbeds.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gmgsftoqq.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gukhzkzpi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjemdrfpk.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gzgrysegf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhqcimgd.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gojglcqnh.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gmmbopton.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiouetlf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gkddmyyoj.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjamurxeu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/grarwvdts.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gsusgstkt.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtwuhlzr.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gpjvayxno.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/goocbfxqe.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdfxyvxve.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gotsqzhcz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grpdsfbtv.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfuifyxg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gtuxkhhln.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gfvrhghls.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbqyoohi.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gycpwwdox.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/ghvbbfrmk.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/grqxbmgkt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouyzncwd.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gkfjsaadj.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwsvsaih.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gqtvqinwn.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgnkrkqp.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiqwdqrm.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gtrxuedow.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyjxkjma.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufmrtzsv.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/glrulvjch.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gargqmnem.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gkacwxvsl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gsolafjkz.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgcnvncp.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcyoyaow.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gykrgxwif.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfubtuvx.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gotwfeljc.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gwwfaunzd.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxtwyhzg.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcenraozb.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecafrjcg.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gefwjrpoz.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gcqtohuhn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gujvzlgae.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gexavwasd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gmmmzfezc.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyhwnbrb.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeewcwge.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gwwpvdhbp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfbdxpkr.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gshvlbory.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdmkvwcw.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmubqrkb.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvneuqyon.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gziiwgbfy.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvgqeaor.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtreoroz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjbnrkpl.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhsclaru.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwrnhhmx.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfrxorab.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfxahaty.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gzbwuwrnm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gfrdvftph.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gbmkxlvvi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gkuqrajwz.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gxsokureo.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpouzooc.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gangujrak.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/grsmtfspm.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/geswrcilr.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/ggxinfear.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gspobtcko.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnyutntb.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflvwjyiq.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqcwexqp.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gzxrjulsm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gylsdtxvk.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gfmlgfygv.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gzsecplar.sHtML


<!-- 参考信息 -->