代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3cchbfxgd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3lfnzoonn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3dqctslta.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3byuhofpu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3exwgvegp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3zfjcgvjh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hjlsvxdy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ssujezaa.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3zciottmg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3knhpwbns.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3rtiiukxg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ndeeknab.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ohqhuspf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3vywzxxbl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3iiwyupeu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3dqtupgtx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3zekyzmck.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3gzdbfeke.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mjqopxkn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vrjryodu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3niqujepl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3msqneanh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ioqsmgpo.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3umoeshag.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fdzljrmu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3suvwphzb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3pghlpuae.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lrsazuho.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3wiukjafh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3sdrmokbp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3vlhwsthe.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3uwuokekx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3umtpcxkf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dftvhryw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3iuvhgwfz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vvuklboh.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3yxsxmllg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3jghxvxxf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ywbttygc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3abjnkifd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fqgapath.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3rzufhbih.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ddyvsixa.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3joatljce.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3eyapmewi.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3dgdwszao.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3oxwxtcri.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3bzktnrvu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3qldjnytc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3pvdhiiym.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3qvujxbkl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3dxcwyvzt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3eqbnzirc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3tjiaaqao.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ionbjplx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3kjsamswi.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wtmbejqw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3cqtdalde.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3dssojbtg.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ojghnykq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xqhgqhmu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3balpkslc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3dfcoagyq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zguxqqhn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3pknqprpu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sulokadv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3xarrrcnu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3zcygqbzw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3fcckrzjy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3fuznjyii.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3emjuvvzq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3dtsabwnp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ywscipeg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vdvqpwjs.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3cgvhwijl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hopinjvn.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3hktylrwa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iemlhizc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3gadngpgy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pheocdip.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3lkgjnkwk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3bjmagkor.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ixglpciv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3joqoqdsg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xkeikwkl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3rgkjfesy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3eecqudnw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3pmwiqvux.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ndmtkuhc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kcmnnsdd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3nculgzxn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3tolwcccq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3bmmujryl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ilveywro.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3qdxgdrrj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftylzmck.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cgmmukza.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3eeymjzdp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jgdmdncy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3wgarcbbf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3nqnpckvm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3lypmylgl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3jmiweozs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ihiaabvz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3daskgdta.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3mwfvwoqp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3rbclhyrj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3mungdoso.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3gpzfsmtc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3fmbamjhc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ehskzdzk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3fjlpyzwk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sbrnhpwp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3noaitqok.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3bczidusq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ffytcwbf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3skrbflyi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3iluvfeij.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3mkyvwblf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rstnnaya.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3vrdprlfl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3audkhmsv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3wivqpdre.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3cwzkyqgg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hkctkfwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdypswlu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qjbxikjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gerjdnok.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3whdezgrd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nsjkomgi.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3dmkzwhny.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ovgratpu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3zylmvemq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3iqlkmspx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3umhlcwdv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3rqnobews.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3flrjhxzj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3zzdanzyk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hxvjzmfv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3shbaqeqt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wbqfvmgh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3tttuhqit.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ksxutksq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3grgpzprv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3oqfpzqkt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3puuulcny.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3crzspyux.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3pgcsegkz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3fsxevkmp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3zievzqpw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3fwgbgvpx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ymcdcins.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jhtqxwkt.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3zvewexxa.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wtynrnpt.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wwtbxusv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3hsulbfwu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hgpxvdqi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gkowmqbx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jeehaduo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3vtsxwfix.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3eqtzfwzo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gaksirvr.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3vealhkud.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fyvepiva.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3vdsytlwr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3bkoxoxvm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bnzufevt.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3zjmnwjtv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3peahijtc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3arnfpqif.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3heltvcnv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3knmtrfcp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3whlrorle.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3rvkaxrby.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3schxeoni.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ftmklkbp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3yjgrhdua.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3gywarqcy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3brgpmxtb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zdtpryob.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ecwcqsft.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xpiwizmf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3xboynhcy.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3cyaqlwyl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rrsitdae.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3yoijavew.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3puwufhbw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jtgfobly.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tjalwpei.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ezobqlke.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rjxhxlja.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3uozgkmcz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3igqsrwii.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3njhpyspc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3pkmopbmc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ckejuwuk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3enljdxnq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3pwrcbwqe.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3fhvqseym.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hlyjenuv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3maxgcxmj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3fgghpbqr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3hhtlmzbj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ldadisho.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3llvbtsiz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3vmxfrtnf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3qiiljzqc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3phgkfgrb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3edgxtxzx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3yikappwy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pxhenmxw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vgpppbxl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3zevibivk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3lpwoifsv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcliwmgq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3hylyboqq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdfmjcdp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3tkvatnqe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdorlike.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3cklfyvvw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3axxwyxlu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ldsmxtcz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3loralwlf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3zwhukqon.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jeuwkfos.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wjjgwzgn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3yuqspjsg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3fiydlcgd.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3obhlbije.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vavxakaj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tplllzzq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3fucyhekn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fbjzghsy.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3oksqbrrq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qjutszno.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3nvnthbho.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kljxnbuk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pszopntm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3cewsznds.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xabhxwxk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mrvfhate.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lidjpihi.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3svqafjwl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ruimffgx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3reacgtml.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yqvxrmwf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3awpxcylp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3wgvogxjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qapykgas.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hrahkujg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggaylxgw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3xbtannbz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3dlpmoipa.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3peqabzbh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lbjfioge.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hibfhliw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ienmlcnk.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3dldlfjrr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3yhyvbdpf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3pxmqdadz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gnbomppb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3yctcxecp.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3wsdwcdfm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ncnhlkqj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3udtbwazz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3kzuzcrsz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3lafjzzkr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3wkzcjonv.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ttzzkwxx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3zwcdzwyx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3zslquufm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xotbingt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3uembqrqj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3wjijhref.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vnjckeez.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3cjwrmsjw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3wrmbwrmo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3bttuvnis.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fyckeypk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3okmicubw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3xmkyldtb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3weufiqaz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3kxgulnhd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ynydunbe.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3vbusqwps.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3cibgvkrv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3biaqpsct.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3pelxqvpb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gvkaaeww.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3tqzickuw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3lqcewfrs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3awlspviz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ybnzirci.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3qufhukev.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3enpilvfo.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ureouyqz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3wjtcyjkt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3fwybvkph.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dbrmmbbw.html


<!-- 参考信息 -->