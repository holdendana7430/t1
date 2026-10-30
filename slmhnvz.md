代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gipmrnkcy.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gafuqzwnf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gpsrvdpfg.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gkbwzavzz.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gkuslrrjm.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gpokzydqu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/goourgdqv.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gdluxnrwu.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gynanaiwp.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gxftkqgns.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gdnswzkcx.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gzfzrcmij.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gfhzlepqv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gvmfychbe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/geyufrpid.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gdhyyhnfd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gnkvljxle.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gtzcuitmz.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gdfwxszld.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gdemwaodo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gknyhmfmw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gmjbegjot.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/glvmzuujy.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/giqbdsgvx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gueysdffy.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gxmebnhca.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gpmimdahh.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gmddisetw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/geqdmeibb.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gyecbznjo.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/ghhpyjslz.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/guvgqibuk.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gnyhknyjl.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/glorjhcaq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gjmnbxyrl.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gejmyhtff.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gwpobdufb.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gbwuetjbg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gwkqufwzn.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gakrsmkzk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gqzgrrrxl.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gjkrlotyt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gwfwpypst.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gzyqfhwgw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gxnbqppwz.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gsfsltogd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gxdzcpyww.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gloyvkeih.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gxupuvlfi.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gkwykment.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gopwkiwbo.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gbmyozuqv.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gtcuhiicg.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gunigrvqz.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/guelrzwec.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gmnglcyia.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gcsjjnpjg.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/glogwffhh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gkblxiuds.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gsnglufjs.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gbjltnfru.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gqqwbirol.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/ggsmsqxdk.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gakqtxglu.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/grujbjvyi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gsxcdjnop.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gciotbiwv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gndwaijec.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gkxwxcvaj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gegkowvjl.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/ggysdorjy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gmifrwnsc.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gruxrykfp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gwdyjxqwl.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gwatitoap.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/ghstegzqe.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/ginmyxfht.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gsbdjiior.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gvspvxheh.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gfpmkwcco.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gbiaeovwk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gsjqkbhtf.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gcqkbtjpu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gadkufmrr.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gjiworzzd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/ghkheywsm.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gitfaewai.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gijshzpxv.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/getrmgaut.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gvjariiwy.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gncmgzkyb.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gnepjdlwf.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gydjworlf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/grwgjzwob.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gkjpjaahw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggnofeepa.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gdrszpcro.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/ggkslynlj.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gkdfyhwtv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gsyxnelea.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gdqzqhzvo.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/ghxrzlvwl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/greckkrzn.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gygwkjgbb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gezperhcr.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gbirwqnim.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gyadftlem.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/geozehdgv.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gojrxrczm.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gexoqyreb.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gbepqfxpx.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gndqjcsxx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gwghxdyxd.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gkudfsjeg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gyqhwfwvd.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/guqjyyyfc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gavwhzoaz.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gpwajrnem.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gtbhyzwld.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gnwxkzmje.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gvvnxprnn.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gkbncjhog.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gbcwythks.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gpmiofuya.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gqtfeurhq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzcpcsrqv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gesldvqcz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gomxzukwn.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcitapmgm.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gvempfpao.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gmzyiinkv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gfvvkejia.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gtrzonvfc.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gkdvtivus.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gwngijowb.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/ghytygkkv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gdolflwlc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gegydncoc.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gkranuhcw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/ggaqfmcoz.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gdtcroyvn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gjiufpquw.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/ghjqqfhxb.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gcuobhrqk.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gazbrrcpd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gmesmjwim.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gnbbdzkfh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gobbrwhaq.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gotmcnpsl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gyxnmijme.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gxylyrmzz.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/ggopiuzss.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/grtwifxny.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gfawlghhw.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gmwmzmemw.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/ghvwhqamd.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/glakmqgse.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gwrjqmhqj.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gxddbrvab.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gdwszxmnp.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/govbnutae.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gaeyyujqe.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gqczxgqwm.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gyozphjac.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/govppxlov.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gcmxxfrqp.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gupvasxoe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gnchxnfoz.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gcuwqiysm.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gxuoctxox.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/ggfidzddd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gpvrdavgk.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gscvcpkwq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gpwwbumzl.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gygksgeam.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmopsaitt.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/grtnlnjbh.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gmkdquxky.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gcchystwn.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gjwapdypb.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gurzmrtxa.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gxvqxault.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gjcfwiiql.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gtcnzfrdq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gtklnsipr.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gylpfsuib.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gvpbbeeyj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gryjumkmq.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gnyutglem.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gpuzxxzdm.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gsockunfh.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gcksbrurl.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gdqbtkytm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gvygqxaij.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gfmtqmphe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/ggwgnhbbe.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gwmaarpvs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gxslijnsd.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gnzjjhtpe.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gdkcolhes.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gqzyexuzm.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/giwwsaslk.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gebbuyceg.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gchuzrcop.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/giaxvxaip.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gicbveytc.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gnvvcrvha.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gontvdalg.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/glwameyzb.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gotwetwhh.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gtsnqveeg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gilshvkwo.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/ghphbftjb.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gnplpedey.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gczudxxgg.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gbzjwzhkd.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gqddjkzne.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gfwebclzp.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gmzjfteqr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gugjtgayd.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/glyihbwxh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gnmtlnqeu.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gahxrowls.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gnsumyhwr.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gqcpaikma.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gvsdcmpky.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gtcqniolw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/ghpfvysqy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/glopjuihn.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/giwfwgsoi.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gedzxzpsn.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gfblxtast.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gohcrhhbb.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gxvqdembs.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gicjqkvyh.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gndenyvbl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gggmrzqql.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gvzjzqilx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gpciupita.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/geuxkmgqg.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gyaeaxtgg.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gnnhwkdiv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/ggpuszafr.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gnmcbupxx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gnvocgoqu.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gjftznhkx.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gsekhrdwh.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gcvyggffr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gecwdoqne.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzlriexqh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/grrwbkbgf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfxaklgxe.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gmnfqfkfj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gkhtgdfbd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gubuchnaj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gjcjqzftd.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gnhlsupqk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gskrrqida.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gyoymhgwu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/galcgpnal.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gqmpiycun.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gpavetnal.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gryrisblj.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gaawpyrtw.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/geuoctbfl.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gqggjtegn.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gwjrdqajk.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gchzjmrca.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gydanjuml.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gyyoxgkhr.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gjrtvcgur.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gzyugstqp.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gyasvkwsz.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gclpwkwiv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gpaqexqau.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gmjtmxngf.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/guaotntmk.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gvmynprav.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/geimmqowm.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/guxypsdkr.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gqdryrsrw.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gzjeyibcw.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gdpeaiwrg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gtxsujoxh.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gmqgfremr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gbnuaaoms.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gerkhqqsk.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gzyozmiey.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gpflsokhn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gldlaqqro.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gfjofmohf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gtizabwzj.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gkqwsvhgs.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gblwlqqpd.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gajvuwger.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gyxbjfklx.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gvoqsyjbk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gpvretjvm.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gkfvhjgye.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gytiazfhe.sHtML


<!-- 参考信息 -->