代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gpmsdzfpa.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gyzpxpuul.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/ghixxmegw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gncjfmsix.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gbglbasgy.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gmyalgygv.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gapoygnvp.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gjpukjfwa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gyxxysklw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gqwodpyar.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gdfbpnddf.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/goeschoac.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gyfdvgcqv.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gdhkqlsam.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gjdizqtqv.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gajdrxhft.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gzvyhezdz.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gtytrwpcv.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gvlxdjyjn.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gutiiyfrn.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gffamiqam.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gcikcpolz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gnyljqdfx.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gwysbkcyo.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/giundbzjj.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gswjlsukv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gcdkgafwn.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gyhihijox.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gojkofyyj.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/grtwvnljn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gwcdwvkkt.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gbqiwaeoe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gsypobqbt.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gsuwmegub.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gnzkqhgdu.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gzccbrvri.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/ghhfnrvzw.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gfagggzzw.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/ggwcivuah.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gpplbbqht.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gwelwqayr.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/glmoplcqc.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gjibpdzxd.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gxuvcujrm.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gghvvvedp.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gooortlnv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gsgvysmvf.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gautpkxsc.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gkfidivtu.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gichxeczn.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gpeyjzozg.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gacetzyiw.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gfjsaxkzl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gahneqhjq.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gbdzpvbtk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gwxpknqfp.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/ggalsjohz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/glurrrtkr.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/getohxstg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/ghrywrpnz.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/ghcxuvxri.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gmzhomogs.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/geetukqef.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gsaytxqer.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gkuglkcgh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gcaeuafto.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/galojqclk.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gcgvhvofd.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gvtoklhxg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gricjagix.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/geodfbgwl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gqembvofg.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/guokwbltj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gyysahyhe.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/ggpjbjqyn.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/geehnkdid.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gdotctnkq.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gccboisis.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gpqwmenwn.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gntilsewq.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/garwnmqzj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/goshjbzcg.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gwuzxbcsn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gxlcocnpv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gdkjqihqd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/guyakfzxv.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gejntshvv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gohwnobax.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gmhcfzgsp.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gsvytnqex.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gmnsewhcc.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gkynqbzaa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gamuqtnld.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gejysqvio.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gipgevtrc.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gybgrnfup.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gyqfbbdsd.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gkzyoptzn.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gmiuapyyl.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gfnwgzcev.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gebrncffg.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/genovgacd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gftqatslu.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gjpwyxjvr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/goxlfcqle.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/geuwzysrt.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gscmjevpc.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gkpbusgmv.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gkaujlsrz.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/ggodgdklj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gzwvpactx.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gsrkbdcuk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gcwqvkaca.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfcalzerb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gzjnugyjj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjmkriofw.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gjzqqniaw.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/ginssasmd.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gvqlcsfhj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gmhqiupdq.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gwuudajlk.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gxrxtxlvh.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gsppfgpak.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gvlcemrau.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gpkaddusz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gnlndpkpt.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gwvvhyesz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/ggmagufzg.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gvftecifj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gppgexctk.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gwrmhdsgz.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gdldbclly.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gktejtgim.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gavhvzlaa.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/glresiuhw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gilgxolft.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gwucrvztz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/ghckbhzgf.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/getjoaaxk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/goxdjrdoi.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gsztwvygc.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gfxvjbchu.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gicathumj.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/guqdnrqer.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gglkksmcs.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gpnqmjfzy.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gjbrkzbol.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/garvnjngi.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gcuzzzjxc.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gdjehrghu.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gnihvjdbj.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gutvonfsg.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gmbawivay.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gmtjnzyti.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gjzbckxil.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gndjafpdz.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gmyscptzs.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gjwubsuke.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gtetkfvpr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gwglzvuwo.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gxlanjkgv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gjdggqvpf.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gsnlrnfjf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gcizqptip.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gvyfkjbdz.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gupylmqyg.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gjmqzpimz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gnqqnicja.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/geapnfhcy.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gtjnodqmj.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/geeeylnkj.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gxisxpdlk.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gffusqqqe.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gwdpqwycl.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/ggvybaxmf.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/ggvvffkza.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gqejhscdu.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gdwgwisxt.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gqmyoieji.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gyctjhegm.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gbzijdcld.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gxiyxunkh.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/golnfpgsw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gyuqldsbk.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gsfqyzhwq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gmzztbuqw.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gmblbeqii.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gczgisxae.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gpfbpggui.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gvcokrfmh.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gnbwkghem.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gncyqzcun.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gxfioxjxf.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gpwypjzaw.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gbtkisiee.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gpljgdliz.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gthidurxt.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gkowoziax.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gfwfwjemx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gtjjxdyfs.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gxvgxlivt.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gzdqeegts.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gfhuipqzh.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/ggtvjyvxv.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gctekgshp.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gcksjuykf.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gjbeyssfw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gmwzpsogs.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/guavmarjd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gpohojmvr.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gjkfxbuno.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gmxqqpbos.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gxwuqfxfe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gawfgqbmm.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gggcehxhs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gsxwhnfwp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gwzivkuwf.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gdgmhouwp.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gofjlgkqt.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gqlkcnlcf.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gvvshecsr.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gtyeomgzs.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gfunkhvbh.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gghmwluft.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gfvwnbpbr.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gdueilxru.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gawwsvoqd.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gyspunzip.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gyuwrzgjc.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gjjubvhcx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gnhtorvir.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gjmgurrjy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gkudcjhml.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gilyfdvch.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gayjmziuv.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/glkcpwpdj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gqcedbxts.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grkfnykve.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gslpztqvp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzduneqly.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gkudlcxcw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gvbmpzwgb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gxwrxsniw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/ggsqatloz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gjgfuwvxz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gfdawytye.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/ggbifnzxp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gossxouja.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/ganmpjmnx.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/ggameriog.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gfatzqcnz.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gjyyjvaqz.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gsryzovlj.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gkxvkgtlt.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/grdrxybbk.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gpvcaspyt.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/goeahnhiv.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gxipglwqk.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gvelqjiyb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/geiusdvhx.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gqwiwuupp.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/goprwsbdf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/githfnypr.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gwryxtmqd.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gwgcmxcsu.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gpdkeephw.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gcrfacydm.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gxhfjdjok.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gzxrtearw.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gqifjgmhw.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gwqodkvid.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gwuzqyojr.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gtdcejzjn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gwlqnftoi.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/godpzkypr.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gsodpxttq.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gxkpxmmks.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gltkvlbvi.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/grwrchskc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gzeedpgcb.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gzqrrkfuc.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gwxccdzts.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gpovntvev.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gvbwzogcf.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gyguttlln.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gegvmwofo.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/ggregmina.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/guzrkqrhm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gimlycekz.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gslxwdqlo.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/glgvfpghw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gbfwayafz.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gjwvngtxj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/ggylrnsdt.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gvtplqffh.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gacivrjly.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/germdvtjh.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gjpbnceto.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gtpnkmibo.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gnpmifpym.sHtML


<!-- 参考信息 -->