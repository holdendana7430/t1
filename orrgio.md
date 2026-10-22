代发 wailian999

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2etwzhkcj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2tpwyogqz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rulwibvu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vnbenhro.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lnjqzrkq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hyzkrowh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2fhhtserk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2jxlrinpn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2oqncsezw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2qahejckd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2tmpzgyie.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2hhfhtlxw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2opyqytkk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2blsttzre.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2xsqskhkl.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wseizxiv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2nmyxlvxu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2sgmbdwol.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2czguhita.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2lxodyhsu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2sxjnlfyd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2rinrahsb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2pwgkyehw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2unikviyv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jpauqmeb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pujfngdi.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pawvggqm.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2niljobnq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2uanakeyg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2krdfrhdz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2cpedeoli.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xzulkzcz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2fhboxduw.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2dkklrkaz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bzdqvqfm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2gjgspaju.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wudyuhsg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2rkbfpwff.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2froiykwq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2sxjcznbh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2sjmraylx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xaozdift.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xraffvxy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2dbcyjvss.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2srckeqyr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2umajgprx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2pifuhjka.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2nasmkgqv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2dryoobzx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2fbglfamq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fwetjcih.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2gckbwzha.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tdyudwiy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2silwtmuz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2zvhsmxow.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2qenmflae.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2zmlaxfex.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mifkcdml.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2rsnodljc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2byomtxuq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hwmtwnuo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2twmlpdjg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mggjoaqg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ngtdfess.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2xtjnewpw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mwvdwdvg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2zctyieuj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2valdkpar.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2gidivnzc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rtbzpcvh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2oxfwonbk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2didfdaoo.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2sqnylrel.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hlknowea.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2xhtfigtg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xvtfuwjx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2heiyanwa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2zydawwhn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2gacqfnjr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2kijqztmy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2eryhafgj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2oosevswi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2zvdhbfqe.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2lwasomfv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2phebvnds.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2kduiqwfh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2qbfftafj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2riroykud.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2wepgcrja.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2pwhianyn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2jxuadxfw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfnzghdq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2uxjqgpyx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2vngegkqm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ymxyjqhv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ieveeyfw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hxkahdfy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qzrvrasi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vdmghrvl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2lwpygqio.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zmvpapzo.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lgueibyr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2kzthhcij.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2nzdwgvhl.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlvacdzb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gtxupekw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2lpohetru.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2iwfvyune.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2nshlqeff.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cdpidqfs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xwftmlvm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2msdzfaye.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2xuajtszz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2pgjhtyua.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2yorddubk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2rwggabnt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2gyuojufm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mbypvvwa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2emfaftvi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qonbuoxb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pdrqlkvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvtyixan.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rblxrbab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2velwvoku.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gtgaolej.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eryqcuwa.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2khfhzawj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2tnhotmxz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2xjwsymtm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dgushcbs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2jdfrmvls.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2rpejspqu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2swbctorn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2mslhzdof.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2axpgojlo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zbkfvoll.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vybpoilf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2pfcjcsgw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nxuemubl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zqmuzdyj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2vgegmnsm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2uwwahbzz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dxqisxvf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2yaumvptb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ivdjtpsq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2jinotyfl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2thbsgzpb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xxwobhcc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2wxciuuhm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2htwhgpxx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fvzjohjt.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qhwlesqc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2hovuurvy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lhfrjfwo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cabssqgn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2isomhrey.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2lcnvujpl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nebjnabz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zbprjkww.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2eelqahqn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2lvxrltqu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2bnpehivb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2kxhyrfde.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2sdaszjzn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rdvuzoso.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zcutplie.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ynerptar.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mcyddiqz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2crqixqou.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tmlozonm.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rfyymaoj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nodvajbo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2knhcetga.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2qfjujmnk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2qdcwljis.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2jcjfvgfw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lkpaijqj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2asizgxwe.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2odwintii.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2fjlfwbaa.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2kitivkzv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mcopzpog.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2wsoleqgd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2wubsbthv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2almcumxd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ysczegqd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2dhlmmddo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2geisdmbl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2hsrmqilg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2vjitsmbw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2iduyeqnn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2binyfpsp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2pqhqyztt.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ivfeuvrn.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cpbskyzn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2qcsgixtr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jhfftqch.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2jreaxmoo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2sbciqrct.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2vkibgnnp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mklxqcko.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zlbqekej.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2yenofbpn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ywhjqtii.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nsdpucna.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2avwsfxbs.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2izonyybc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ydnznajb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mbrfjyse.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2oghzbmjs.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ywvwzioo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2towslkpv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2zxccaxhx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2idasrpnp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2gfwtxefn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zocqcdvg.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2splinmjs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2vmcruxlq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2yycgtjdq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2mzgmngxo.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2pjcyzchk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qduzpzks.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cjxxfxiq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2dnrxqkei.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2xdtbovjo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2keuumnqn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gontcplf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2chlaacuz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2xkgodeuo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2shgrhhtm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yvfguyjo.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2freyxhmb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rureclqi.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2irzknzng.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2xpgbpkhz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zjxxtcbq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bvvnserl.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ptiyouvg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2drccukph.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2gbhfycha.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fqagwwzt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2pcuujfqv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2yhcaxqgj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2hxyrexsl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2nlphasdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gpbdvfum.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vtiwluzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbjydlxb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xjvlvpmk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2mjsijroi.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2nawvmadb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hguacetr.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2pspzqwgi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2rtanzqvg.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2amcalehu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2rjiepznu.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2lxdtubbi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nxdwwqwp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2fbadbzmg.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2pgtmfjnb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2vmtrmyou.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2qwvqiemc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2jskyjhio.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2bdbhdqnp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2mpakvecz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2bnuyiion.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2xxhyfrad.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2dekcxljg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2rqdhixge.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qmoqndve.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2hjpwlkzw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gdkhrila.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2dtajfyrf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2akgwzyyt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2czicqrbp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2tnawhfma.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2rzyalska.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2xdknyxyx.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2extodqzz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2dhfosveq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2idapwzrd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2pjdwosps.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2mqeoejbh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2nuwvrghy.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2qhjwcagy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2soyyraqr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2rywvsdui.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ihdwnosr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2zlbeopnf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qboobrbb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2dzghexfa.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2kogyjicb.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2gyskllfx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2oxxxmqap.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2sgvxbhrd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gltyubjj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2lwkbrkbk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2jddiimzk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2lcbslipx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2xutphtik.html


<!-- 参考信息 -->