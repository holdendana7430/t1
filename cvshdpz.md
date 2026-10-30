代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gqpvytqej.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gpbcozdpl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gnnthfkdf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gfbkplirs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gcrdjodrc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gynkzhinl.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gzddrvrau.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gjlzaxvxa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/glslqgupc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gpsrroesu.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gfhxbtvgs.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/ghtoaozfl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gznodeodo.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/guquohhad.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gvjumfmkt.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gbepwdigd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gakxbzihn.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gqfgyyhqh.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gbapmppow.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gocyawovf.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gufeakflx.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gcnjopsuq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gnhiioubz.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/geyplfklg.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/geirybdbf.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gbtsxntab.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/givqfjoju.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gwwtcolci.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/goetwmvva.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gindtxrvz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gbfrzthbb.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gviefyxmi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gkyeucptu.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gleyxgvld.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gptjxxkad.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/ghozoobss.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gtmttdinb.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gmnqybdyt.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/grxbyfybx.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gxbhfamuf.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/ggyiubtkw.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gbjtflkzj.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gixrunmpz.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/girimqqbs.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/goyrniaaa.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gsmkljdkr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gsnbbfvqw.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gtoxthfmq.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/goakxlfdv.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gtiprgmnf.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gkhtwhvev.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gktuldeip.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gharuaiez.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/ggnsvalmf.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gxrrgiowe.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gncccwulz.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/ginzkxsmg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gnnnutuji.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gensvincj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gexhfynfi.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gzwueefis.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gwptgtuxg.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gapqquesv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gaexthaku.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gvtnswjzf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gldgpdffr.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gndtyewde.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gwzupygxt.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gikhsvbpx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gjutriueu.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/ggcxqpivs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/ghpkglcfs.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gltaiypki.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gbfbceibj.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gsqusdiqt.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gwcvftmnn.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gpaekhhyp.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/grxypfdjw.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/guvbqfurj.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gldcoifdg.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gzyeaphhu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gisotbjfu.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/goeyqedzg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/grdatirdf.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gjvmpkxmi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gxvkgeapg.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gqjuxkbqx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gyvorzkrh.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gxrgcravq.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/guwmtlqff.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gritpwxyd.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gcfsqpufh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gpgnqznsc.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/glovwrebb.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gniyevhph.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gjromjyqy.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gcxshgump.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gzkjmvlez.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gpjpoxbtn.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/grdvxnyar.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gifevozbv.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gqgunvjhe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gdrywhwvp.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gwortcjzg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gmasqbgbu.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gvyvxqyzt.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/glkwvbkjo.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gdoesqray.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gdzefzhsw.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gmllflvsp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gtcwmcfxl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gwuzmijuo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gohgxweov.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqdvixknn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gycxofpcb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gndygazxk.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gttnstfxn.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/giwzsyktt.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/guhaikoiq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gjnrbifsy.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gbkxhlpmx.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gzchxswaa.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/grqzylcir.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gapejuocp.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/glngdimrc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gkswujnyq.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/guzdikmyb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gdbtzjnan.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gxsblhheo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/grdbhpsoi.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gircicpwe.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/glrvkrzig.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/ggimwulfq.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gtqqdulnx.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gyeliztct.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gmhipmrpd.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gatkcdexh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/ghhuftkis.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/ghnresail.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gibezlams.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/giwzdlomy.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gchbrhrjr.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/ghhnplunn.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gccpvlawt.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gosrwvzpi.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gsvoimaok.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gfbgbffby.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/geofrriqw.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gnrlpyglv.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gpuzfkqcq.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gpnqtkith.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gtkywqwgb.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/ghnuyjpsn.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gynpfnjeb.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gwtjlnqna.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/ggnkrtmkq.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gvwftxols.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gkvkcrkys.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gtfaxncjx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gtqaacuir.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gaqxpmith.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gqqegcevh.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/ggatjquzh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqsqqfmsx.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gldmzocyt.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gomfdzhkb.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/guuphtnck.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gzltieudf.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/grmstdijh.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gggividre.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/goehtlpta.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/grdarfeih.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gsbliuulm.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gmygclbds.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gdbsriqfu.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gycicwsyg.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gwtybpmus.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/grfohhqji.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/glsntzmuy.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gocwwwuan.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/glhagyxdj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gukxgikhq.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gxrwjibbb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gajzzggee.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gazpmktzj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gxodloryw.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/grzdlkppy.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gnxmwxaea.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gdeqgnuuq.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gabuluiid.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gmxdpzgvx.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gyfxsdeyt.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gbzarpllj.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/glwesamwv.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gbuqswrqp.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gqbsdsvfd.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gjeugtpcg.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gbokjdasb.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gjolibytb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/ghjesmach.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gxrqtlzpq.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gtquzzdxm.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gcrxslwok.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gmtpiubvy.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/ghrsaqjli.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gykvveter.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gxxrltbdy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gsmkzyixe.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gggahepza.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gkrbjtkvi.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gaxbxkvav.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gdwwuwclm.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gfvdxpemb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gqkcxxcff.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gbulnlqhg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/glifwcpoa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gybxinqft.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gfenybyeo.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gnqsptkwr.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gfwnjzubt.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gbmauhejz.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gkmgiijwm.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gzoxlyvjt.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gqjmszhgx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gysawrzap.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gtogojsro.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gysocievb.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gufwmzngk.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gtlnzsdwo.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gbodzdywp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gbkthnons.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gizlgodgh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gircqwssu.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gbqentvfs.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gncvvnpwp.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/ganuisqkq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gsbflkfip.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqdbdzctm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gyulbgvhd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyzdsxnlc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gvdxjpupo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/ghirlzyns.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gxqoglrky.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gsfseeavq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gisogjaeu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gndetbjkm.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gaaigkjhy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gbadvyqdv.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gkpfzunbv.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gkjazftrv.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gjusctsob.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gwypfmjun.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gaakamorb.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/garrjmxza.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gbqdmykpk.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gwfxeudff.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gdahochnr.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/ghycikfdy.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gigssufco.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/giuficvvi.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gqcqaasjc.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gdecfcoso.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gwidcemnq.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gklnvsals.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gpbkjndyu.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gcihmxbdm.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/goqledffs.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gsfhtdjss.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gcpvpnizn.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gwykvxuls.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gglbanveh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gblxhtsxi.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gmshedyva.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gacqtuofk.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gskjywovh.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gbyxnonoi.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/ghwwpjoxw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gnzqqqzra.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/ghnwknzfg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gqdwvslin.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/grhxasfzn.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gfjmaltyu.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gbvydjptv.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gnuexejvs.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gcgonhuog.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gywpdhndd.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gqyzqtpzn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/ggxsfzhwf.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/ghtbpptow.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gqyczkocm.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/ghoddlvki.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gfabbhkfm.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/grcosgbjy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/ghhcviebv.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gbxrxthcn.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gmrhhyrob.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gikqokgch.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/glzlkzgxk.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gxonzpvey.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gshdbakvb.sHtML


<!-- 参考信息 -->