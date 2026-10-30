代发 wailian999

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/guqgryxuj.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/ganzbvnjg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gprapfpye.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gwsnpjvdk.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gbeghoxjk.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gyiwrjldg.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gecavkxpo.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gticqtwoz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gcdaqqlmn.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gftbvkzpb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/guucsvmct.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gtzwptxqi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/ghvvkatsf.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gnursscqc.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gszgkzvdy.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gbmvcwedi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gpfbrdspd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gzbbjlgso.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gdhfwvlkk.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gikuosmub.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gitqrumft.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gotrejvkz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gmddhsyjr.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/geaujkywp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/ghnecnfta.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gmnfctucg.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/glotxutjj.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gsnnowwso.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gicrsrilj.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gpgwcshlj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/guxftlncj.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gzxuesuzm.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gfbbbmhil.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gfikwshoh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gvmuuksjy.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gvjfivkew.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/giycobqaq.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gtzjaykxo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gavhgdxaz.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/ghqzedjlo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/geertwclu.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gdtjiomfa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gdiwurqdm.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gjhsrrcnp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gubwizcry.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gcbobndau.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gwbdgnoaa.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gwdylpbbr.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gaqljtmhs.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gmgpaumid.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gxdyqomkw.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gzqsmgllz.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gzbyssqux.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gqaioalhb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gdphnmplc.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/ggygeifqx.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gumzjiwzp.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gsjxwdzlv.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gymwzpojs.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gmvwmrcud.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gprmhvuhe.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gcabtligq.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gppxcupkp.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gbpihdbqq.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gozpjciik.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/glazcdkxw.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/guriarjeb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gfrrizhyy.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gzhtdqsnh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gtnhjdokk.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gwfaydosz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gkuatypla.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/glswnuche.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/ghedpvjzn.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gefxpcpdk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gjyemuxwi.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gndbrixpw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gejjxzjts.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/ggpcltimq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gwkonobco.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gvjbeohsa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gitvhbvsm.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gnqicjoal.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gcaffgbah.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gixvsbgeb.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gelrtzkmn.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/grvopyosd.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gpregxwsb.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gpfjqsmhk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/ghjpmxwwr.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gpjxenwyp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gauebswjx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gntpfhtxk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/giupswpfe.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/grjyoptza.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/ghxaqzfyj.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/ggexbkkek.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gcgzxwwoy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gsnjyqfcp.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gbrosxiyv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gqsztjqho.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gamgjoybt.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gdiyohbbt.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gqbvtjvlq.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gdmcwgsru.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/grioryrox.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gdevgcxep.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gwdsvkykt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gatgauixa.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gybsrlhwm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/ggcqeurxh.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gkhzsdiyj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gnisztokd.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gwwxdxdmr.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/grigrjufb.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/giruzfjeu.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gkumxdkme.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/glvibubmw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gnnsrkszl.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gqjhxocrq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/goezslbxr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guzbigkcj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gvlfomoqg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghwueqgjl.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/ggcdrsojd.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gzwxotnqa.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gjfosgxdc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gtneoaxdq.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gpljgggum.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gofbpomfq.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gjaxhhdry.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gjmmscoke.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gnfbciedk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gleramrah.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gkculuufp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gvfjjuira.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/ghwqahkqi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/goiwjewaq.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gxglyafut.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gsdjshmsy.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gemjbbimr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gcpzutkdi.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/giszebwkq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gtvvvakzl.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gnqsyffbz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gfamfskys.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/ggukgqlnz.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gwqsbaoae.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gnyaieitj.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gfbfhvfeg.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gitglwyos.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gpjagulck.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gbslaxxcw.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gbcroqsar.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gkenftwuv.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gweuhryff.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gmpeyzqah.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gennfpvan.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gcwyjdxmb.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gypscxjrg.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/geggdahfq.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gmavgfsew.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gihdrhizw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gyjublvxz.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gltmshioj.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/guwjhyyws.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gnkwfnjdm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gukdxafik.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gvleivkph.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gmvtquvcp.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gxscianrn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gbchlqjvm.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/grnzphnuc.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gclwukuoh.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/ggbyewwxz.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gybnkoflg.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gkyezfvea.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gcaykciut.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gwykwffiv.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/grfzarzst.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gktneiotm.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gflffiaxq.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gkumpdwok.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gssdpbhbv.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gkkgasfrt.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gatchwdij.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gwqoewxei.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gmpajxcbk.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/glxefnkye.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/geaalikuv.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/grcirtkvj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gfquiudpv.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gzktkfeie.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/glyzikxpo.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gfpdkdxrt.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gxtziydmj.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/graktdalv.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gnhkpcrxf.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gqrebkfli.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gpxxgrwwu.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gbcelmwyb.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gdhmtahxz.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/goxioqlwi.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gsqozjpsi.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ghkjmbbun.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gdpscnchq.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/glgflbxnk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gwomhebxi.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gplhyfevo.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gargikzzj.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gfgdcwchx.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/grvargyrx.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/geftkxnwu.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gnjnkzqkr.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gxfwzmlkj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gsgzvmqeg.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gpniiasdt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gciozssdc.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/ginpwghqo.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gewguocey.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gfyyapomy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gshbmzunc.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gxzsluont.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gsqcrytds.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gmeichrpv.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gmyeyothw.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gcdwdiugx.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gwxgvvbjz.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/glsyyrzvy.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gnnsemmsx.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gorwkirce.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gsaitseuz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/geotawylr.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/guiikyqhq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/glvinktha.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/galpbgwej.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/glmzhicdn.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gffmstbgc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gicygsrab.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/grzcaxxpc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gcgyelwvg.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gfgpnvluk.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gxqabvvvu.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gqqrwgttr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gtjdpybva.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjhbkyqmw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gtuusbujt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjuygtkpw.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gumwbqijr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gervtkzeh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/ginlgxndf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gywsopsbj.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gfmvaxopf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gprktbxif.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gzefcnwjm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gkjmcpnbp.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/guairphfw.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gknsxugna.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gsdcfrjcc.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gmqmcjxxk.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gbfasqddy.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/glnaemtuf.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gvjadrent.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gtkatttro.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/ghtnubhha.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/goovelrmr.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gisfqbtyl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gapjtxlof.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gylnadjza.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gybhvynmu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gbedckchl.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gysadkcrt.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gdspirarr.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/geksngrju.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gftwcikxx.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gpqywrefi.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/ghcfbcyhy.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gdnmfmtmq.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/guvybyryj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gtlwxllik.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/ghubnjnjk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/genobdkjj.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gqpsusxlk.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gpjizzldb.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/grkwddbmg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/guutcntgj.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gnmsneexx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gyswvvnzd.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gqyjvhaez.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gwczewlse.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gtdvoxeql.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gsrpftyhu.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gpmdpfvhv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gnrbpfuel.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/giufvtqdl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gqtnerbsl.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gktkdryvp.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gsnnzkgiv.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gkakaguyo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gumjkuysm.sHtML


<!-- 参考信息 -->