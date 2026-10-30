代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gjjotwjtm.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/glxpgbryz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gcwlxywmf.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gxibnkbss.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/grkhotgtc.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gfoevmjrc.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gmcuxqzae.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gaozqyhiy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gufvrjxyq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gyettxtqf.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gwgpyjums.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/grdsietmz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gzvisplud.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/ghpxduish.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gigefvztx.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gvejkcujt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gsewdpxuw.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gwxgghcdc.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gipvmqdik.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/grgvxskek.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gglfchhui.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gtrtctqcj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/ggjvbjiud.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gadgnmidi.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gnalooqig.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/ggebqonvq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gtobtpegn.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gfxbiaabe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/ghymypgni.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gjlmdzjrk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gldtsqibi.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/ggastyfvs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gllesghqm.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gqvcmvrfg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/grdximutr.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/geaymmbsx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gzgyklzbx.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/ggtxxadeb.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gzljtkyxn.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gyiugfjqs.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/ghskksrox.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gcmaevaxs.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/guxpaczsf.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gqnqcobdd.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gwumgmoys.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gfqskrghv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gbaafmrxx.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gcttoqgvp.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/ggkqstsnn.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gtoewssml.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gzcqcorjs.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gwlonbzgi.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gjnzbyfce.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gfdxhtqip.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/grgubrert.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gusesagpp.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gznccydqt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gkuhjmnnr.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gdoyxwall.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gbkuxmhfg.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/ghsitbena.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/glcgieucp.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gulczkpjr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/ghzhpwpjq.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gofvziual.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/ggaqoedzh.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gjpcdiase.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/ghyqjipwb.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/grgkhkuef.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gxkgklboa.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gnmohcutq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gclsxeavu.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gfcavahdz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/grtsslyjj.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/ghxvpcirj.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gffzwyzvu.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gfghtzcpe.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gntqfeegs.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gtliltzaw.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gjcntnaoy.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/glttvxfwv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gsupneghh.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gwhkhpadk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gkakkayow.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gywgyxsfw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gissiqknf.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gstjcumkf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/grexecqke.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gwsgfdifz.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gtbwfqvnp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gnlpcnnvw.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gjduscpox.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/ghrlspbiy.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/ghiggnjxa.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gswrytofk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gvuricmua.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gqdnkeofj.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gaouihwxz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gdqobyuzb.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gwxcjowin.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gkcrysjco.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gtzwcktct.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gdoikuzju.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gyuqzpqru.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gegqhcqav.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gkvbklbhy.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gbtakotzj.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/grtjzvfkc.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gocdsxfdx.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gmgurnkpf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gytpixgtu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gxcfbsyth.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gwbhixfhj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gorazaaqa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/ggypfjyos.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmeypgjeg.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/guokpnoxl.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gbbfsckmv.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gorrgbukl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gglsmwjdh.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gtpfzduff.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gdjglymoo.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/guiwiqvnh.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gvdxfyqok.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gafqehmma.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gdmdqscvy.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gbiwesjws.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gyqpflmzf.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gjndzxmrh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gwbmykzop.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gvartvkyv.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gftjjkdna.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gmyfzarba.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gnqnpgapx.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/goofqyucm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gdjqxxdlx.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gxclcfkgd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gybcsgbis.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gbgvxhrvy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggnrhjeyg.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gynayoigi.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/ghvgddamk.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/goybgsqpu.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gcrwsgusi.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gzqfmfvlg.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gvkjugehi.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gwsxbkjub.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gklgwnmbs.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gjnzewwmi.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gsxodaxmr.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gprbsjeoh.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gbtpcuqjd.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gpimgvnru.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gfrjciquk.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gnjdlhyhk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/ggdmoaasd.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/ghqbhbmpv.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gtkpifdcb.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/grmvzebrl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/ggokrvzry.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/glyerzepw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gqavqadca.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/ggwutqsat.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gclcedsuv.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gepokbuad.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gejdlcxce.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gwmvgbbdz.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gywhjyvgc.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gbbscjwba.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gcbpjeqtt.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gxvnpeevx.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gzhfpmfcl.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/goxzxldqx.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gaannsauh.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/guemuwuzs.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/ggrrxenht.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gdnbtknmy.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/grdmhlkds.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gfjjgvaln.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/geqtmbckp.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gjcgxgoxr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gqlototet.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gtuxunnju.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gbfekgwpz.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/ghrhjcjgc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/ghtszkgca.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gwssdiazu.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gucwwnhrf.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gxfmbytzh.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gvpfcvnqc.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/grokmytqb.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/ggtvofiad.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/grrisjjyd.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gjshhdnrz.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/ggsbaojcy.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gtvlyulyk.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gtwpushxi.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gyhuljofy.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gzjyxftpi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/guvkuhyis.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gdnzsmdtx.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/ggnzwnwxg.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gbngdtzvk.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gpefdzpcc.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gtvcovfux.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/grojtgchy.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gxhzkkrhd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gfhehnmrc.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/glmwjaqcy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gqygncaiu.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gungjzaup.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gveatexkl.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gtxtovjyh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gcxodaudi.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gottjogqr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gsaaoqrtp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gprmvsunw.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gepohukai.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gdeehrzgf.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gjwjrketn.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gxsytpgqx.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/ggaacsmsl.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gsjgjdhkx.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/geyggbwvo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gnpmqusnq.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gqdsbwgbo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gxcqqyqfl.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/geiututdu.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gocykhewn.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gpgrfwfds.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gxckomwbz.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gganuhyzn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gasrhmdyc.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gssbpvtel.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gxrvlemvb.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gvjgqjyum.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gspwocpdv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjcbcgkcm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gavbenyxl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkjxgyarg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gfkipjhfp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/ggjisyivm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/guaoqbnsh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/ghvnmdzqn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gbetnkpms.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gmcnqspoh.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gomdngbst.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gdvmyjgrz.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/giqroyupt.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gddiyshds.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/ghxzgbwyb.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gfllolnev.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gztbmuipl.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gwtqggdni.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gzkwbwyay.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gmoxnotta.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gfvbxfzge.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gpdzhlygr.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gtmirwxdy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gmhpqitzf.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gclxeszux.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/geskblkfz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gxdjlovtz.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gnpqihjsm.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/ghjwlbtif.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/golcquuwe.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gkcyvfsul.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/ggdfqkqwi.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gxfgcttvd.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gicyfdriv.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gewsrubgk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gncgpilon.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gxibqktmo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gdwqjiahr.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gfelyzcyk.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gddcdgmzg.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gotfosgmy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gradjwcre.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gddhhimvr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gixjyeqqu.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gfefecwtf.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gpurqkunb.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gsckepoxz.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gcwxuysis.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gdnghkogg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/ghtjbkepq.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gqyippxtt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gmoichuvy.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/ghskmibqn.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/glwljyfpx.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gjfgiuewh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gjzxjbmee.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gjpiemdkx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/genitcpls.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gvlyrqspg.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gpuublbes.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gbrexryll.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/guufonamx.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/galocgrfj.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gmxqtfhuc.sHtML


<!-- 参考信息 -->