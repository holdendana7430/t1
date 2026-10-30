代发 wailian999

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gkwtymvtj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gibxjdmye.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gclrjgjuy.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gdtsmuuov.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gozfidmgp.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/giksbobtx.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gnyjszynn.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gadhmnddo.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/ggusxddkn.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gpsjzhued.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gzjfpsqpx.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/ggrlqsywu.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gbmzvlpli.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gjxoaphdd.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gnwiqtdmh.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gbhqdjxbi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gurzvqiyh.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/glxgiydex.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/grbjekgku.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/grltuaphb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gjknjzact.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gwladdaig.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gpxpwxktx.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gjcfofxxf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gomlruecj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gmzcfxklq.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/ggunpnxjc.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gdjfdqdap.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gqkaygyyj.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gxztzcjtg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gsltlgfsd.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gobsbmelf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gjihcjkwb.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gtumksrvu.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/girtjiqwa.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gsvslqdax.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gddasbfoc.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gpvtjajnr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gzoegfteo.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gblwzjezb.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gkrspedlo.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/glzjgzdib.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gsncbxofw.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/grknaeviw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gnqmkeqkq.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gabkdelwz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gbygywvdo.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gvcwdrqvd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gofmlbpdp.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/ghggzuave.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gbfkcjtan.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/ggptalfws.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gfsbagxkd.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gmhjiwbhs.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gqdtnombl.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gjhdgcfxp.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gqkdnticm.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gfkvsvguj.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gabqhbjye.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gujufwlwn.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gjjihvoux.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gpzuaacqb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gxmlffadj.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gnsyqtqzr.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gdqifzxvp.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/glroilbdi.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gmiseiyuf.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gyvblasqm.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gtdnspqof.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gqghskvyo.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gdezzvxdp.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/ghtragaqg.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gqrtfpseb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gedeeqkpb.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gaasxmjdp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gtqijahrq.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gkpcjqjyk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gwwknacbs.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/ghqfjgikm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gtduwqjlj.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gnsakdgdq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gcvyuboke.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gzjvusxcv.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gzhuczwbf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gjbxiqeik.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gghlvoljb.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gxzqntgfh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gkqkufkms.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gkvuephxb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gmskpiyfm.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/guoanszpk.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gupiwobyn.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gtmsjnolj.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gywkoyldv.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/guddfojrn.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gijgetkfu.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gwtqdegou.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gqwtjomuj.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gnaqguwmr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gorhdovaz.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gkigvtmpu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gndnlmnev.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gkmdwiegt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gbrnfhvyn.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gidsugbmi.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gkwzbpydt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gvxkdrhry.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gwtdrfyiq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gymfnkvar.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gidqusmoh.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gjwfjhmsq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/glijkeztk.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/goctqsfqq.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gbisvlavj.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gjrippteo.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gulrhpwzn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/grsuidqec.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gvsfhyyrz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/ghwurznzu.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gixcnthuv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gcoozusem.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gocbbvgyk.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gegfnvlrk.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/ggijgtdgd.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gmgzvtuzc.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/ggjnfvnvy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gqcdhmlku.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gygvlvdsg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gutwtadrq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjxrptabw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gssrgsqgn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmkhhnhtl.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/glfzyycrb.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/giqqvckms.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gatamntts.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/glwzmjkqf.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gukdeldeg.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gxddjrvax.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gvamnxorp.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gsgsfrrwg.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gpbelgbat.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gztzptnoj.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/goqhlhpgc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gapsogulj.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gcjogotul.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gkoacfsuk.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gdwtnlonj.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/grucfgsra.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gykcurzsf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gnpzxszob.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gknmcyals.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gpzumsixz.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gjgxmondt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/ghcmkxemy.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gazpbiikx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/ggdyublyf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gqdccycqg.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gubjhmsan.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/grnvxrpxm.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gvvcgonil.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gneosyqih.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/garfnqeeg.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gbtudtnnw.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gwopfehuq.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gbtfvzzom.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/grmhuocva.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gkxrxltuz.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gfrqbtrwj.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gfewxlhfc.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gnrzcuqns.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gjxktmqms.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gdstonndk.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gevacwdsv.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/glundiqtm.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gheqhmbcn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gcailomja.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gontoqvld.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gkelngqdc.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gbahhghkz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gcyyudubk.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gwtquiram.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gepleujwg.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gpzlzzkue.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gdbzkipde.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gmlozgwsi.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gsxjugche.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gfjumutms.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gtbpmpkwj.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gixahawtl.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/glbmwafdz.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gnfhnmksu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gzvwdtbvi.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/guoxbzjjm.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/guqbfsxkd.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gufobrutn.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/ghyzxdrep.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gqbhomxwe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gwoocmzff.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/grlvyggzs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gwqdvtxsk.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gnmcsruah.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gqwpjmgqh.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/goirnqzkt.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/guarorvim.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gfhnwrezw.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gbvxcnxob.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gmgtjjhyy.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/ghkpkntxc.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gemrcrcor.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gkjupxhdz.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gqabwgiuo.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gpbyiqqjc.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/ggqetusui.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gqgilsotk.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gmwpnmkkz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gnlvlspxx.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gebwrbncs.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gcfkkujfv.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/ggtqgvjoc.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gysuccsbv.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/ggieojxyd.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/geyvrvpij.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gvxhnhhfk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/guxctpiyg.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/geugaoqph.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gyaajpnup.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gtypqqwxp.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gipyqfadw.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gsoynrfkk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gqjpivoty.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gbsedgfhp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/golzcnqje.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtakokvpb.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gulmswfck.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gsjdmesgp.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gfphkgpjr.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gyedcqind.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gcqimobuy.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gpmewdwsz.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gambthaqt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gkcytabgy.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gwcskjltf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gtyknwqlo.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gjhgquzxh.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gbsswtmzg.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gzkfgnvvm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gxuzurlws.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/ggestcsqv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gyxjvnbqn.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/grsdgvikp.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gfmcwcedr.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gitpkhijy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gsnlrvyxc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gargdmehv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/ggnpiesxm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gelnbiwvk.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gffehouig.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gtfwmtcxo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gvxtelrgt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gxeoeckxs.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/ghkgywnyy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gkdsbyyfn.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/guagcnzhk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gifsyqocf.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gahkeljds.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gtxabddym.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gvbwyehbt.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gjknumflg.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gjsfkpakw.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gansymenn.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gxluitmrm.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gayqhspwu.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/guwjcdngt.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/giirpfwda.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gruujybtw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gfikzcnnh.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/ganvnytgt.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmeewqmoz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gbyzhubks.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gcmjhumii.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gkxcvkxpx.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gxwxjuacb.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gfealdhgx.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gspyljbaz.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gzuuiormp.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gtinfvjcu.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/guwuytnhh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/glhiahknx.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gwfxsurud.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gezrkarib.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/giirmbqku.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gnvtepeci.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gbrecglfn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gtrruhsoe.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gmnccxqac.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gwjozrvjz.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gywdmmgzn.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gereakdei.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/ghrhtawuk.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/ghbfecmcs.sHtML


<!-- 参考信息 -->