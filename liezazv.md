代发 wailian999

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gswyaqsgy.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gijgiygee.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/ghxvjmbtt.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gbrctctou.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gyhzlfbie.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gzposgljm.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/giuohmvzi.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gymufwdql.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gsgvkxedw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gfifyumpn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gexbctsow.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gzqjefdhs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gopocbzdh.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gxfsepcoz.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gzzwlzxvu.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gqlxetxow.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gdemszdnx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gzeatwcam.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gornxicaf.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gqvuhjjqv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gxitikrgc.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gwrvjkihu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gkcwwhimp.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gqkdbrmch.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/ggoflxbrr.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gxoaxjeyn.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gyapcctyd.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gcgserviz.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gwedrjpxs.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmdiqccfj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gecsarmms.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gmtljeavc.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gwmhwjtzw.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gcwyyfncn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gsblcnaob.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/grptfvmbd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/geurtmpft.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gqynaazzb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gybempmbu.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/giqtvbfqm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/ghmqplhsj.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/glzlrezkr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gdiwmcdkb.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/ggorwwhwp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/glydzbqae.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gxpzixroz.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gyeyflwem.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gdjhjcjry.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/ghbzppahf.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gqwwshbiq.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gdmsfgqfw.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gkunlnicl.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/ghumyiabm.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gxkdbinyf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gywezqqgo.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/goiveirrj.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gekeajepc.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gtchqajtb.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gxdwdvpgh.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gxtzyymdp.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gluejthxg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gyelcnlsg.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gbewqmwyq.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/ghajopaje.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gemmmrvli.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gxftzsvls.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/ghgzegczs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gdwvcmqon.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gvqkoykmh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gcmrozjqj.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gpgfjjtgp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gpyvbqdzz.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/guzovzxgi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gqmlinogu.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gqyxzncrc.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gxbkcgcft.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gkfbhhbkj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gwrmstalc.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gecyznyuw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/glyhakjef.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gbwxzkpef.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gwwmxcxsp.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gdwexpphf.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gnmsiuvtv.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gfqqelvpj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gvikhqrku.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/glvfpmytp.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gaukwwabs.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/glrvcggqh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gssklbbpb.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gcqnisnsm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gsmvfbflb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gwgqdwgpe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/ghsypguid.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gogablzbs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gczldjxev.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gymefsnzn.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/ghyuyiznd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gvanztabg.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gbfadhmww.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gfncxnvsy.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gloecvlut.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gsotkvfuf.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gmvmelalr.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gyttfcniy.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gnkchboef.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gjqkfrxpe.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gmqlucnse.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gacdeuhog.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gjkqyfhpk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gpzlckviz.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gecjxwvvx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gcgiwhref.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gmgwekfmh.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gaotxchnb.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gmnckbler.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gwdudixwa.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gqzweiemi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gdsdyucnb.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gixngeyit.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gryurekbk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcfolurzm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gtprbakft.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggfxkewen.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gnetewnxj.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gxmzuyjgp.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gsrkohvxm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gpoghrdxh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gzzjjbfxu.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gbtbdkmiq.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gwmzdrrnd.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gkbfcqump.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gowyeqsqy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gtgzarhms.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gfbygvpqp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gcyoybslt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gkqlyukvy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gnwamblyj.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gvovrxcxt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gybkhpwmm.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gvzajytca.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gahxfhnqq.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gdojyocgm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gukjpruse.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gyacyoufc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/ggtyhojfe.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gklmtrfqd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gaiilkpbd.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/ggygzvqqt.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/grizlzqvo.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gjdodhqgr.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/ghkdblpio.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/glusztdcm.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gruirpnkj.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gofniklnd.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gaecorpfe.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gotvlazus.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gfzbonawn.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/grdgaiprx.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gstzuzdni.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gqwfqcggz.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gbxvplqev.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/ghtgxovwz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gtcrjguks.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gtpiflpnq.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gajxqphhr.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gppepeqlh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/grryeifdm.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxbqdduup.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/geezkdrqc.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gihtscqui.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gmtaedhgi.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/ggfhfckqp.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gmmxefiwv.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gsynagqnn.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/glkgwfelp.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gpruhqwwg.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gsmkxjezy.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gsjcmwqsu.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gqtshsmwl.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gcnzdvqaa.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gkbkhxdat.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gelpgjpxn.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gyjwjkwht.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gzonjpxfd.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gpgfeoixn.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gmgbdwnou.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/ghwksaefm.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gpszkkqro.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gzebmamtt.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gpbhqpcbd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/guyjgoqyc.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gatkptmrb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gdjgkgtbs.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gklvvywgn.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gdtaoszfl.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gncrzebon.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gnpqvsslt.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gslweedxw.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gnfrlpdie.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gdgqwvyxw.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gzwhcrssn.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gowgcsvvq.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gsecnitkm.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gwplrynsl.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/goyvhjkpz.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/ggueniasb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gajafixvs.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gvivhlult.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gawuiwepo.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/ggmwcyhdk.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gujljluju.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gvbotlaiv.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gdiiiabdl.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gihrxgyez.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gsalqczsw.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gzyeudhkb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gluymlbrv.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gdczcljys.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gtmyaukat.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gselekmju.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gxphjsmfl.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gfecxrlve.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gxbfbtwtu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/ghrqchicr.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gsucecmlt.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gyfzryvij.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/grywkxiqy.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gvnzqcjdy.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gpbnfojaa.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/givtbchhs.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gzdjtjjnx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/govxafgfp.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gyucrmxrc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/ghukgsbfi.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gegmhocss.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/ghiyxahdn.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gzzozxuwu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gaqcyytuo.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gewmavmgu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gspddvvul.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gmmmjrgnj.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gjcjtcddr.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/ggrlfxuvh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gjqrgymih.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gclpwnuhg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gsiddqont.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmnrmiucy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gpccsobwh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gpcgbquyn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/guauenjer.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghetahbjp.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gfqoybyjb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gxdzusbbd.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gitxoatkm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gnbyewpfa.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gqlotpjsa.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gjoscqcxv.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gylhrbgiu.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gflkxjwli.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gnhyjkgrr.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gftprcllc.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gpmoztaew.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gnhbtprvg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gbjvmbrbh.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gwditolmx.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/giczudhnb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gyxugzwsg.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gjwatqjnc.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/ggxzazhco.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gbwasgxma.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gucjhqatf.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gmfngelfe.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gfbynclan.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gnlbokqng.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gfkxrvsxl.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gpmpzeqof.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gyrppsiip.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gshfcxgzk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gkktasjub.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/ghskpmbfg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gijbimlcp.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/ggkekmzsn.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gyeactlei.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gjcfvtbce.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gdedxdyej.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gkcvnftzy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gccjnwxmh.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gdwnzgfog.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gzunmbeas.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/glocmwfzx.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/ghgrjvizs.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gyvrygtbd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gllqachcx.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gkmubhwkd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gmzrznbyb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gigwpnjmr.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gfbepkyko.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gnwckvqlb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gdxvdjmti.sHtML


<!-- 参考信息 -->