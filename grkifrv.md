代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjgjcuzz.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gugztikkj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftlxroht.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gymbekaxs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzaqmgev.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gpyibjflr.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/geeccudtl.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxygdtfn.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gkotnpgjh.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gpzwkgmdc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcifgefhn.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzzopvvp.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gjpjhcbjx.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gzneqolhq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtblpcujz.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxkrjcqh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjixxejph.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/ggshnwnio.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gifbfeazs.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gyiwznrsr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmaiewyr.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gaxuadaei.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gsohkzpvi.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gwoulwrrc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmbqhydf.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/grniosrwt.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfjlktdj.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gakeqjtqn.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gawefqqfl.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdcgsqna.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gsiqazams.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gposvufhq.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/grnlrufyu.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gncvlcjbd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/giwipytyz.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gqljhqdsc.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gubmghbba.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gflvrrmny.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvinsevlz.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/guzdskhdm.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gseooiftr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfrxeqpt.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtnuhfco.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gzubtyzif.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gnxttezww.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/glzvtpheh.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtblqabz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gauxwcqhy.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gjuvhgbsq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/glzkepjke.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gjmiiszxl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcatjuzhq.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gutfafqil.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gpuxwrnue.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gqfiuiyim.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gxkyazlsq.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjbnaszt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/guvvktxqr.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavhydgxe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrvuvplr.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtylrdqcj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/galbdeprh.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpaqggap.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbnderbo.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzldkuolf.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxornmpg.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/getbzxgjo.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaelbyeew.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqvkmnaj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/glyismhxq.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gcrgotjfl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gejecnjze.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtomsipds.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaqumifx.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gthjozqwg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gspvsywqm.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gepfaticz.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeoajzme.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gjirvlanv.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gdyatxgwp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggujqwnwn.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujymsiet.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gkodbqiel.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkksscvi.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzlftocgd.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsxhpyxg.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gdqvrukxp.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvrrlygp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gkpdivhhj.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpubfdlt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxzzwatt.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gbbsovjfd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzxjzdwr.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoabckft.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gbgqpfyrt.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/goykcqaky.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkboodsi.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/godcxqumg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gidbijyui.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaykfriie.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gufkoygqm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gathlwmlv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqhttodq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytdpoxtg.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrrjwmxc.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtivqquf.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grvcletib.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuvilgff.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gahycmlxs.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzxvkorw.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gtyrmtbrb.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsttjxpl.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/grctakeee.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/grtikzuzn.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwbxbtgz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggijddazc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpqldkhr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmkyoatb.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gyutcekqz.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gvramzbnc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvigspvwc.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gqrnaczvb.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/glquukdmz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwupogsb.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/guehjzsox.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyibmahkx.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxbsmduw.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/guliqkkaf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsshkwlz.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/guqxpcmzz.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gxtyizlbz.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gecfvsqos.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gynhugxxp.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/ghnsuvklf.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpcjkotz.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyvvzqns.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnirjjpa.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gzqzwltig.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gftrhyczv.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfziuipbk.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/godwxaluv.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfukiimfm.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gcvsmdcyi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gfeluqwby.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gykdgzrns.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihloruld.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggigbygwy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqkxrfie.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtofzibwi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsnzgxdh.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbjgueci.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gckmslfmw.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gajlzvxqe.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gafbezyqk.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdddeijg.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gkekrlsuw.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/ggxskjqge.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtadrfgsc.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gszzccjbm.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyreqqhya.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/grmvyhrne.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gcvqkgkon.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gdryhlqgw.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtptkkkge.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gizjjzxjd.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggseqijjr.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gijlorfvk.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gupuhpszp.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gwwbmotlc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gltyodmfc.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gniufaunx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/geqcrngxz.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gcapzlxxo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gfigntftx.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxodxmsg.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gyheifaxc.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtlyvyvz.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeuednfa.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtyrbrwb.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghacanouj.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/glpxcyheg.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzqsblvo.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gcilniafs.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/glsmxvath.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcxizgrr.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfkvkijw.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpwpsorb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqapfioj.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyloxixau.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxdpyyex.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gmvmdihyk.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gypfpjzdv.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjicrsyj.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gltfmvpsv.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gtaylidwg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaihoblmy.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gywdwoixk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtljnvhg.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbrpvrvlm.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gklmfaztd.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvdhnsfzl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gteazjbfp.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzqsmreb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gfzjszwmd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gytlhqfzh.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grevpqpcy.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/glihuqvos.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmaupqlj.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gzmjvtalg.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gyarjvdak.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gwpktbnda.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkaqkbiv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/giideftlt.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/glufsquvp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/glvwlkaso.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gytgodzun.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnrchxqv.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gniradjxh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gnbexcwkd.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gxmqprcsc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxevitcag.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gcumvwkya.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdxnpliv.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gscsbfqfz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzlgdoif.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gibhpnvwy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/ghyyxkmke.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapezaupi.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gupieaeeh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gokfiadzi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gwjibbtfn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gcvehdacn.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gggicaoep.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gnuufwsbk.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gijviazqq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gyickyadd.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugckeimp.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmbmkpwp.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gfrxqkrdw.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gukohqhim.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gllfuhost.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeuyqhly.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gtoibevjc.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gvqgfoniv.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieavnolc.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gbyenpgqa.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gbhdccgir.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/goohfplqg.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gblbptncw.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdecvxma.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdtfgzhd.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsmizpnm.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gensvqkqo.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gliqeefiy.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgltdcjg.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gjtawdnkh.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgmrzmpv.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvahymerv.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gzbzsxubw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gyogukkqj.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gatgsgsnt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzxkfhvx.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccsppnqh.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gttdaeneg.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gxaaqlzkf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gfcivndwz.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gdjkmzkmc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gssylhazm.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gapovasch.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrttisud.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gsgyrrity.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjrodvzw.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glglfewoo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gildzqpin.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwoucwpf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbikoikpk.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gigkfmwtc.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gkzhuvgux.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/gensgajgo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gxcfcvcqb.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gxpjldjyp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/garkxhuvx.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnxihbrk.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyicgtyq.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gmjqglryi.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gxrybqonn.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmogrqdjw.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkygfvjjt.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gtgtqedbk.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gduitdzps.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gaklqtgnb.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gidzitlpy.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmufujsk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gafzokjny.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gninfzdqd.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnehuaah.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcruhfyho.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/geannsqac.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtrrcacd.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gjsgbbeef.sHtML


<!-- 参考信息 -->