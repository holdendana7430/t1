代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/glttlvzax.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmigltai.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaofvavlh.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gglooimbf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfhsgblj.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gksymozfz.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwinbsuij.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdjxnall.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gtntrkxuh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gcpiwrmic.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxpczjdi.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyaqjdeix.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/grzznltwl.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyyovusz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkmrligy.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxkdlvlg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/grjdxclkg.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gkdzwjxov.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoocwoyl.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gjbicafne.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gktqqlerk.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gevbjcjaj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjwpzrtr.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaimrlja.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeheclrb.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gjphzgeix.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeltifee.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gjiskkegn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtoiyytr.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcwmzblw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsygnhbn.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gsrgygqwn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfwzfkyk.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukrxzhhg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gurbnwahi.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gpgdchett.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/ggpguyhue.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gazluhakj.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbmafvjt.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gocknzzqa.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrssexnr.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhgbjyvw.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gqicjtxry.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhmxpyxl.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfthhqvux.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlzrutdl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gwegpnfdl.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxbqvnli.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbitnyta.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gampgtacz.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyoarrez.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gdxsrdejt.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprcqssai.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdwcwdcd.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrwmljax.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gikutvplw.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkimotoc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgpwyrrq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/grxjvqfbl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvcbeibh.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gmeuaajhn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gksznmuqq.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgnahoav.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/guvvcbxoz.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gnkqffsre.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gohqbmbvk.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gkitceqth.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkksakjm.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gghcbipnx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmxaiqxo.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/ghyvvgiai.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyiwklng.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzqhiuyz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gzhxjdcsn.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gopdybhjb.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gkrdcimpw.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gmhflqvsp.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gdpsaenry.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gxepnbzrc.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtahuggc.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuomlnib.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gyyxavfwh.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gxpiopxlr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzghtquib.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/godqdgpuf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpefhafm.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gznkerzti.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcushrmok.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gjiaijtwz.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvntulqr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvozicjq.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/ghvsxwztw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/guxagmnul.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyederaqv.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gwqpggdhh.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gazisvlzb.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gohemcieb.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzdmfsly.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geivqyekb.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/ghkepyllx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpwlpsen.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmaoxvsp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzodaibhk.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdlvnqhg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzadmdwg.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/ghqgzqadz.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/grjwsscps.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/glfaoovkj.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/ggvswrktr.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmjgirze.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbydwkmde.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gmpixygzx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/ghizyrmpb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtotcapvd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdeulolu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmugwmrj.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gwgmtuibk.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzrnsyht.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gybzilcew.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/goguuydyx.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/guonrrcui.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gzzppkkks.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclruarjp.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gulrneloq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpwvjptt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gadqxpkcw.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gxjvnqxjr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gngzecjja.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gzdplgpqc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabvgowax.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmalhyai.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzxdmyhu.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrceadzx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmpeqavb.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gguluakdb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gtxsyfjvj.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxvtdfkn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gmnocdadv.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/ghityuxsr.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdwbtsjv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfsgxzwn.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxrsvftt.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gkdqfdfwd.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gipxurixk.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrklwiza.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnavuijtq.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjjczafz.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhautvii.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gweddgvah.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gxetrcqgg.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gkggxxsgz.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmcbrtyp.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdphqvkz.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwdswrna.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gngxzifkx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gufhectwg.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfkeztwe.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkuimpxq.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gilkecwet.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxxwtraq.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwetieiin.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/grxotdmca.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcoerfeg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gnsywjkua.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gixxzpemj.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gfarigxds.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giocfjlwm.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbghdaxcg.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gigerbdvd.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gljnnewiz.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gvkkidnyz.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwscaidn.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmelangax.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gkumvtwph.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gqihxpeyr.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/ghsgqbhoa.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gtanrshdn.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gutgkvgmw.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ginprcniq.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpobrrjg.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/ggrpdxxko.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gxtdqdkyl.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gyokrhfrx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gigelzrat.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glivxrzjy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/goazgpdpk.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gagxltkck.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gfuzoasbw.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsarklue.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gtlotollc.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvighcuw.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gmwqzhifg.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gpibtbqjh.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyndaefnh.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gdssokwdv.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/ggloiuehk.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gahlwmnkq.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gnbylbkyz.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrakirxj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghulhwxmm.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gixjpcyfg.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/ggsffkast.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjaqhmgor.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsxaoccaa.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gfngklqzs.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnaaochw.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gncnepsbh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsvzbpgsp.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gjhdtxiyg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckcwdyog.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gjudzifkl.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtihagyvo.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gshcwgmme.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjtysexl.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gajjcggwf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gauzennbw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gogmrzhlk.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/geqzgcyyq.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gwesjypte.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmexzpyps.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gjuciukbc.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gxkqsusgt.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmeokckx.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbydiodbz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gygoizhhp.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gsohqeqmj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixhfovgb.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaqsxpzc.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmexkucv.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpkuqplr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzuckjrp.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/glejndjyg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gnaujrcet.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gmakqyzsz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqzmysex.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptvjggxp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/ghcszvtib.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxmfkdqr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gkxlvopjg.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvlhozxr.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvopztjs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gugtzqegz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gfkftsval.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggltujbgi.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/ghbihcbbm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gmzfknvvu.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gmhueslxl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbxyilar.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gbveqkqrg.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gynwllqkd.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqfxceyk.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/ginkhbqfo.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgnobciq.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/ghxuhwsth.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeldlehi.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gqykwazhg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgrhlguw.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gysacuukv.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gbyyprfyq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gszoitknk.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gynjmqwtx.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwblwdivs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfolgaff.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/glciaarji.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gccbcifgt.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gxvwpxsai.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyfcojqo.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwttqhjnk.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gqacpjpbi.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gkvqqdein.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjpuxcoh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppbquyxi.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gzujfmdbm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnepncpuf.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfctlgrv.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggubgtkcl.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdsqtdvv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gktyxmtre.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gowwsgjvw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gixuojcqe.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gwoqgrmco.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvilgqxsm.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gppwmalkf.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvkqevrf.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gukhzjpzm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gsjsfdcqb.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxdwodtn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhrtbokq.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gxtslrijk.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/ggynzgxgb.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gynoicaxn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gmgwhqqca.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gityouzbo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/givsndfep.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gutkqdufw.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gtmplxrdu.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gznzazlme.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gnidzujfl.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gytltcnqy.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gpdqxovgj.sHtML


<!-- 参考信息 -->