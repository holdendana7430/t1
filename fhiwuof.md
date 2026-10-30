代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/glkycldks.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gmgivlbwj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/goyjrrtdd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gujnhcskx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqooznzm.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gmsxzxmzm.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/grpqytsgk.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbtvaqwuw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gibnxifng.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gnfmxdpzd.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gzihekpgw.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsvoknmru.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gwnmkrtjm.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gtulpnnfn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrchbxuq.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynfxsqdb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/glntpdfqm.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gerenpwxc.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gczlchjxe.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gekrzaskb.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyupesmi.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gpyjbxdho.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gwpjhtgwq.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/glbmogrsm.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/ghdwhyugj.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzgucnax.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gdtqouiae.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbvmnhhj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/glxbowsdt.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gnihplxjb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtntfajrx.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gylsbmlnk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihfrrqlt.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gguulbeoq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gnfxhpzaa.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gssgpnsdh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gaddhoktl.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gwriewyda.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gqmdavsww.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gqdtamspu.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gckzhthqm.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gbwpicxip.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjrxhfnj.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmqggzqq.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmljmmtm.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvsuuxdyw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvphtbcab.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gwqpodrqq.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksxrcksl.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gbedhswqg.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gurbfzfmz.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgjvoyhy.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/glqpiglrv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnaeffpm.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/giopwonul.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/goacxqtfw.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdlzmgeq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/givbndvzg.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gywjeaxsr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvbozzex.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcbjrtyf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gvcyeffyw.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gzrewjkpj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gazwxzxmv.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaorlemc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/grimsewwy.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgchwpfb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/ghksltpfx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyvbmqnm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdetcbfo.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gqlhimino.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gswqnsnhd.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbyakgcpl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/guuvzzsif.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghfnvjswt.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gkphrrexc.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gturqqvkk.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuheiwlp.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsgtyzjj.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gspichlrm.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gmuxwbvpr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsiybieq.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhhehrap.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwaifrgnp.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gunllrsjm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gthofcudq.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwdeowxc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnyyfoxm.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkjymxyz.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gesjobkfb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyzralpw.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gldgrwegb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/ggvfolyej.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gkywfgnia.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlrivqsl.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/glavtldca.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjbqmpet.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gtwezbkeg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexdwtyun.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gnnhwzoyf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/geovvwzxa.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/grylgkuro.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmharhkly.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbmurtdr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gokfkkxlw.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyhefhhu.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/guiyefhbr.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghorvemg.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrqstdzi.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gukdpyewy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/grtdkbbml.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gvqpgsvvu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtjzjcdw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsevhrlop.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gvrivbzed.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhrxrsoo.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvufvhynf.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpylsyqw.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbzeaspz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwapsxdt.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gpvtjwvkw.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gatmbqszi.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmizcvwj.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gwaijzrsa.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/grgtfhhdc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbkgkoma.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gwwdwrqww.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpeywzsd.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gkxlmygoa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlwzbiey.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/ggpuqktrx.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gmiqijszj.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghgaaftar.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gkqpjsesi.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gemsqupen.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gyfktmyyn.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/grugdxuyn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncagybtd.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gogzbufbz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjluubavn.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gftbozcre.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gjxtryyfo.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gueeorgoy.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gjrxssyvp.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/ghosqxoje.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhirnyeh.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gxulxehxv.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gsqdzmhwu.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/ghztcdsio.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/geskrxjrw.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhmonbdr.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gmixdcgiw.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/grkhfbtil.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/guylbbxfr.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcccksen.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwehzysir.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvcebwdx.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giphsnvpa.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtdwclcg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdxavvky.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gupyrxymt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gcwhemudp.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gwznptwyh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgfgcvff.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gbjqivcab.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaswpwsy.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gjitzqbcx.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gevtspqkx.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gqbyudujm.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyvjdcdh.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gebxcqjys.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gddmrltlc.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbzvrjnp.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/glyniizrc.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkcpvzhe.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gjokudwth.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gcyntowvm.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/glfajylvs.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsceuhsp.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbstsmhji.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gqnibqqbw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/geoxntvuv.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/giprkcbhm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gagnzgcvi.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gnqzughrz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxirbtew.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gheqaksnm.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gvegrexaa.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvdwoirp.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gfjqawnoa.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpwzcysd.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/grfjqvafd.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gebehajfx.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gikcndgmd.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gmfwbpszh.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gqegicqau.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gagwvfbah.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gufyahnwf.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grldytpgd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrvcjlja.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvsyiodj.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gffaefpvk.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gpqcwrkqr.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymtclpor.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/glwgiqyzg.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmqfkgogv.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/glaixgfdm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxzedsuhz.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzrzshpz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtrehkfk.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuairban.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gueailhgm.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuctzcgb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnpeugkb.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmoqducol.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gnvvysxkh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goghwdzkh.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grujmyluy.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/givupelnl.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gjjtcydkc.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggutmnbaz.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gacilksji.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/galfriyoo.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnueptdu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/giueweyvn.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gbwldztpt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhrxnybo.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gdywdvflm.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdljemrmc.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaclxyer.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gblghhxdt.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gspegcdzv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/giujjgkwy.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucecdvta.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gtenctizn.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduanndwp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gylhswuap.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gigiisttv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gwxjadetq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfgyvwtul.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gqxhuwvcs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiggeeoz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuowkxye.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfhrrbde.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gnyfnoikz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gatubkryx.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklnhacnx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrqzgehc.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gljpfnmho.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluhaddru.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczqxusca.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gkbaeyzgl.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlthaqhl.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgdgdnof.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gvihrdlif.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/godraeztv.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gabwwfhee.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gfjlorgff.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gopaalxht.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gsjmuwmpn.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgxdefwn.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspgxbwfk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmglmlrg.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gmpygtzpl.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gdjanwmlw.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gdimcbvxa.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gfrhuioiv.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvxnsmag.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gczvbcwtt.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gkcgyjnpq.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpymeazz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/ghowhmiom.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gftbsetsa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwhfdyna.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapazpegd.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwtodmer.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrdovuwd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gtnlmviue.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmklttcw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/glfwpqvql.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gkiifqfzl.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gowwwsvom.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gdcrnncvt.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttbczmrh.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnixfotxp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gwcbagrtq.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/girhuzmvl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gwolmjqdo.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gvlhicztd.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gqwktkqrc.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gamhshhpn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/grmdbkbwz.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gnxktjjlh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebartrta.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhsvloin.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbmpzkuj.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/giiwaylpy.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gdhoeuucv.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gyaepfhlc.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gfipptnnb.sHtML


<!-- 参考信息 -->