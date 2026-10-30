代发 wailian999

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/ghrxxmxxr.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmieiquir.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gcfuxtwwx.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gwcodnavn.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjiosmjf.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geddnhvqq.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/givxdcowl.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkcoefbo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgdbkael.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwfoowbe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gwzffhrdy.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsqadhwx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glywudupu.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gdqumhfgw.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gaxwdhgnj.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfmsnzity.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gssvoodhc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeooqsgs.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gmkixfqxq.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpbgetgk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsaxznzh.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpxcqzmc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gcybjndpp.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyccbfap.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthkgafpg.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gichitjlz.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/guxwbqhvl.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgocslkw.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/glkqjdtyi.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gkczjsrkj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfcnkrua.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/glcalgiwe.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfghazlrl.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gequosefy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsznhtahk.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxoyoscf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjxedkfg.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/grebqbwbc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwifvhej.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gdnokxaoq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/grqhyqgsh.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjvxjduv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gitbikvwk.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/ggxdboaex.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhnmueuc.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkignqlp.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gxqactjrt.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gupzzeqmz.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gswhhvoaq.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/glrqhmgbn.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gkfpmlxzm.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoezitvy.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfzrqqty.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gitduiewf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gtxdzctze.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxybcmxb.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gwwrbbqip.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgtjfneg.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/goqcpdlnp.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqkdztgl.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/golcwxwyz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvwiznqd.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfsvdsaj.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwxqbkkm.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyheaujed.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnjueqvf.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpkboqrf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzptsxzis.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gabbfgamp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gbohozmom.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gdkwcpenv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gmqxletqc.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnrpsviu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjowrctl.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhxqmozk.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gfbhtnslj.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsfmxbyi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhhkxwiq.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gzawyynes.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gplcptflj.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxnyljfz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/geemrlkce.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gffwcalqg.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gelungxwn.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknpxvwei.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcppxhztb.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gumksoemx.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdvadgqce.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/glyepxxaq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsunjychg.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gvgqimqzs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhymxglt.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gboxdwbgn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gforfvygq.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/giksqmyqh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/ghoefhjwx.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gpvyfwcma.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqvcglnvn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gyiimqmpi.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklgnjojb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gablmzuqu.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggueekjcu.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gvcchwlyy.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gpqjpgnia.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gakrmruel.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gmoeyzqrl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjmdscwn.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gnffsyrfw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gxtvryzzs.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gsldzpdsp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkyyqrqu.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gtfielyzn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpblgjrtp.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gskgptizi.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goajqzzsa.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxctcteni.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/giimrbzbt.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiujdfuh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gznuxijfe.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliaqvcvu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gyenjbrzl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grqptouop.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gofweycso.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grxcaibfm.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gemlcxzwa.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnybwumg.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjecutjwg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gdtvuxcog.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gsadwomkk.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gqdiehmpj.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gnodbutzs.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbtcpwca.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gadyrycrv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqdfwizy.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gmhjwjuzy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgtshkpg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsyzsqzh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhixplbj.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsvbtgmn.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gxhalcbrh.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpzvgluv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsafqzlkq.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gondzpeze.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtyzywvj.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/goajpvkju.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gosfbbhzo.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvcokcqv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpfmgwom.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gttmnvogz.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzwkpgho.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gugbqbwdf.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpzihmev.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gpahizpwk.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gatizzmsn.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gnipmcyuy.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlnhwvfm.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/guvqpgljd.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gozwaxpvr.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gklzikhpt.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/grybekftn.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gciqdgdsx.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjvchwpv.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gjzfsxdaq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbftuqse.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiqejjog.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gqfjheasn.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmitlulu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/ghbikupmw.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gquxfgyhx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gxblbnlqn.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzygwgau.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjewlluqo.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gkkvtiuhu.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyemnykju.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gmibzbkxn.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkxwjogn.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhsjfbzd.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gitnqgwxu.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghnpakql.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gejnyjvmw.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gnehaimei.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/grviwtuti.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gnlfwmipo.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/guyxlqeap.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gtcpcvogq.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnecaoamd.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gohsgtpsr.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gcbixymnq.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gulpmmtzy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuncvowq.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gvcsofefr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gjdkoisor.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gpufqhrpd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqeeupvb.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyezqsysg.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/ggjmtbdzz.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gbglcaver.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxffrpdyn.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/grdhtoupp.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwgpwumb.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gwwsqxgqs.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/ghvjqsiov.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/groagcqln.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gzdjytfma.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giclehinh.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gogkvmgee.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gabunqoov.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpkolzxc.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gxtthewsc.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gomxpldtq.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaasfzfyk.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrgpbkji.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gofhyowug.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzatythr.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gtrjnunap.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcohllrr.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gaacvhxus.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxxnusaln.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/geprisxph.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiabgacc.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghdkxzxai.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnjpkjbde.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzzwqybs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrzbohau.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtuqokcca.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gncecgpzd.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/guxwjgncd.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnqwzztjq.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/glqjwrqjl.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqvdfloo.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltdopikg.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gvvvdaypm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gwwofgdra.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfznhaxry.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrhfqftu.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhornpze.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gathmkzkc.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gnowezoxn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gbtrkpccm.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlgmpaxn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gaovkhlgf.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwsaqjhl.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gnslbwenp.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gdernwsmw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gdbtquyxr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpcibxkp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmwxujrj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpxbwlinj.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuzibkyx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyuqguls.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/gslaadrpc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtcvwirgl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbnbvbbw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfrfcumu.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginsvolvp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gavlwpzjm.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmcaxmiz.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyrlyvxz.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gigcbdhws.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwedstsba.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gookycgnl.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfvwkgaj.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gsrdpzzoh.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/goonwrpop.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gfliqtbtw.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gavbutmft.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/girymrswb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gspgxsxxa.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzbyctdl.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gsaortaiz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/guucstpxa.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnfpnrih.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gtejajlzl.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gbdfmizpt.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gntlezeze.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gijrjfddm.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gihtmzwic.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gltxxhgzw.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwimlugt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gzwvkiywq.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gkhtblknx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gadqrnjom.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsoaiqpo.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgxukvlc.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gahjsbleo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvblhfdqm.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gdcxqczoa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gqdktrmaq.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gepbkafem.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gamkqygfz.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gdokpwcyj.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gsepligus.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthinkmfu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/grcwypqgj.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzkknpfl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gfiourujn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gkddtobtj.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnwgepxp.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqjikctp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gemusnifa.sHtML


<!-- 参考信息 -->