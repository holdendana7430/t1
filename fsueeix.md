代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gsdmpybge.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpunulxgj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdygbxlh.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gemsdzwka.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfbqvadn.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gqivseaiw.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gqimktldq.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ginqcxxiw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gmsyiqxdt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfcpavlp.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gssnweipi.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtcieclss.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gicbderis.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbgwwacd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqbekpbr.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaalvcmn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwkeydhh.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gswhionvi.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gilmzirbc.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcmloris.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gaomtvopc.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwbdoqrs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gsjgcxoxm.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gfgrxgoca.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gctorpbul.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gulodvzvy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gnrifsrix.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gqjzlctgr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/guntjoede.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/glbuitcfz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhwfwfuj.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfkxvdtl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gatsoanjf.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gqtggurkz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/ggilygygk.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/giflhxelj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjknqcns.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gflmhoauj.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/growxbtqb.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/giakvvmli.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/glghwlfhd.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gtimmnlsf.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gggwttsts.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjtopidh.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjpwtwld.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvbsnxcp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gztuvndlq.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbmhutvm.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpxiajip.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/ghddlqech.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/ggxmhlplw.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gktjjkygs.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxtvnryj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnobrjzxp.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gtlxqgrrb.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeihsetm.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkopvmgt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gftpvhlqk.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/giitivmcp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gesdwnyus.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/ghukwwtmq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/glhjkcgoy.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gkzkixcia.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/guuwuxtpj.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gerdhyjxf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gniihydld.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqvbtbec.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gffcdiwpm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcztaunk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/govkdddjn.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoclmftr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcepjyti.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbpiptqo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdgtcbkx.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gloohnaex.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gnrbhgnpv.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gylhbpykt.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gehdklcwq.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldvnjebw.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guahwsimb.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/geebtobff.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsxvjade.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gevbzwcmy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvteeccbn.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gctxlhgbz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goirmvbyi.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyjexyvn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gnhaayujc.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gjvbqplar.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gidogjest.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnihordt.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/goametcig.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gygmirbcj.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gwhjdsrwz.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjmqhyie.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/ghniqswie.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnkqvjfle.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdvivmli.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guklefllx.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgygxozq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyuzlqni.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpudwiqo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/guyxarwcm.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkljcyne.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/grkwjezob.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmphtsst.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gbrsuwfpr.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gudriuvdh.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gdexizcui.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gypkjmydj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gefcfiddt.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gwrlqwxlk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclqeohnq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvtxvvxry.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gpojatkoe.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gleglnihm.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gnocmfelb.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gbccfqzxy.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsotdikd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gibvqmmih.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/ghotvmbze.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdembzlsw.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gfggeqjcv.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gctqaeudh.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gciqvnvxl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gwokyzwjf.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxxepkqc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcggcabf.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/ghigqamzi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gnpdiaazt.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gwgxdtgxm.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gisfkrumy.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gofoxkttg.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gedorhfyu.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpabdwxsi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gygvpzcwg.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/glyrgyscd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/guzvsftfp.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gwfnnzwox.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gogvhpmst.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/grgerbaah.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxlskjht.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaokrhkph.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmbzdjmr.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzpwitzo.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnppcwgdb.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gyqmqppxg.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gisedsnai.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/getvuskza.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gtcjbopnn.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gkeefcbkm.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmejuoiob.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gjutfxbwe.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdztmmcml.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfchlzfb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgofxaqo.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gzxvfrkee.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvepicyic.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gadqqyupb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcyriogb.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/ghzxmgrip.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpdpxawp.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzjxbiox.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/guwjfdgez.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gymossynf.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gnbjouvpq.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/grivsstoo.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbxekvpq.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gquawvclr.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbfcfhxx.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gdlxzofja.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbrobyvl.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gkbsyvjak.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gbrvszjmt.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/glhmfjaoy.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/giyrqvdht.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxrjixzh.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwlkkopu.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrqnrsss.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxgoxstv.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gcfkmrxve.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzvhnltd.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/guxsnvyqr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/gzrkhxomq.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gshdgxrcw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gmwfuyecj.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/guynowbjy.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gpztxpkrw.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcinnsmy.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekukauid.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gwtmhysyt.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gpsjnznnj.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfiadvde.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwwdpjfu.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcsqzfcp.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gviuhqhnu.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvswlmvyh.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gleknoxnm.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcqtokdv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/guhcrqjcf.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/ghkpbelse.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guytmlxbx.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmsemeiw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glykkzewl.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gnnxwwpum.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlmnvpfl.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/goddatgge.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdbitaln.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gnipilpwc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gekwdoyha.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gujnpzqik.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbbpgztp.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gygleowkf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrgxpguq.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrqexmfr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gqotfzhqa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhnxpxth.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gmjllmmfn.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gswltdwju.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/grbdzeuzf.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmpbzumj.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmncvixq.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gptfaooiu.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/ghwpvcldl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxihmzdlm.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwgohxqd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gptbuwdug.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/govpoajfp.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/guncbozuj.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gxrseqlwe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmbqerhe.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/grzbrvady.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehptxfqy.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ggscdudjd.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/goaiebppw.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/glagvktgw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gomkrqdsx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvaqzfho.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gcewsszpk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqthlqmz.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gvqhlcmgp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxiayubk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gaspkxkwa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvmjiqjue.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytsgofjx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gmdnwaffb.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gejetzaqj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/glvqsypvt.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseldgxev.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/goahejzvu.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gnsjoutwa.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcxcfong.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gfurhhzun.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/ggouwzaor.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyeavwaq.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/grrypzlgj.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdjamnnj.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpsbonov.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesagwngv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakwlrkuq.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gpihqdvzc.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gadducbvp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gljgxqneu.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnenlywdc.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/guiojnncb.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gqmltmxwm.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gwgmrtupi.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfmmpbne.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gshfnfdbz.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gthvvbxdm.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqnzssuk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gojvqwsio.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkzwxtgd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gjyfegbbm.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gcobrxdvq.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/glmnxwrdd.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuzyaxje.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gotbscbfa.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gayznfvcm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/givoohoes.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gneigvxak.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gweqnliof.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gzitqgjta.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gqlohtiws.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gljupvksg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gyifegvxy.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gahvqmhyx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/grxvccljm.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gzyflgzjt.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjsbovki.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gyryrihss.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gegleyxmo.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gghnkhwuq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gyhstezpu.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gmjbzmkmr.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gcexaydmp.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhkxkhze.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoankvzl.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvmfvhkz.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoswzotv.sHtML


<!-- 参考信息 -->