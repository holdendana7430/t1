代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gfqagcerk.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gciraedtl.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gbxzyhbio.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gkkkmgvvm.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gjkdtwbdr.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gqfgtlyqs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/glftpaabt.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gwkaxmzbk.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gugfyrlhc.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gebfwgcen.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gqfjftwnu.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gvlnqkfps.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gmoyjcccq.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gaasqzrbg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gtbksiddd.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gpesxudjt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gijtexmne.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/ghzhpprvx.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gzjejyfvq.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gcgynpkql.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gcuwzdkpg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gwkotuore.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gvjwojekn.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gpkpdceeg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/ggwnqdaoh.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gfpbkfyuh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gsyabwsxy.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gyzgthpbt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gmcgoaeet.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gwkurygsr.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gbfkjewyi.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gcpdsxuex.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gqjnajcnv.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gyepkplvd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gzmchdwul.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gaikufloj.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gufdxjokj.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/grutdmtzn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gzhnywyqx.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gejkbjjax.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gheyvwaao.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gozlpamze.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gpmnjifyg.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gkaocmkhe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/ggexjzuol.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gwbimfihq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/goqflnvqg.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gijtrmpbx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gbyyyztgt.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gpxjxcfup.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/ginmfbzvk.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gopyuqhnx.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gtdspzmnp.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gpvfryoju.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gqevjslzn.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/grabdfego.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/ggruvzdaz.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/ggpzsiaba.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gzqpdqywk.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gygogmgiy.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gpblinqqr.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gekaxjrqm.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/ggczwoqdy.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gdwhcmggm.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gycydoqeu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjkzfcccs.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gsythamei.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gfnwwkwmn.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gpltimrvb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gbubeffrb.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gmhfffpxu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/guowkppom.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gerqzyjqt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gtsaqkfzf.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gygzuoxtw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gmpvbjarm.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gnyxgxybp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gkphjjmvi.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gigvzrpxw.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gyaaknavo.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gianyyusl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gxcrtudzp.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/ghjwopxqc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/ggmihthaz.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gsfiadcpx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gkpofosbk.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gjphpnuqd.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/ggflayamx.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gzmywuzew.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/grhhmkhll.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gazacqndh.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gzvdkoakf.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gepursuxn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gsllnruop.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gzktpeave.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gwjiufeym.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gfxgzurry.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gjnwuzwze.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gvrbtingz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gevqgqbio.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gxbmdpaxy.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gndecntrw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gpaqprjur.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gjhaslleg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gulupbtxe.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gsxeboims.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gwfcrcndy.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gwvamxhjm.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gferdpmdp.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gitcktoov.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gojbmcbdv.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/goaehzkvp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gaxufdlmr.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gefpcrkwu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gzyhictkw.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gvlhcieym.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gvfsoyyag.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gglqhblub.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gnrogwkwf.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gsbaluyoh.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gcfusaeoi.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gzgourpoj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gtfajicpa.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gofqlktrh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gmunkrjsd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glncagifz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gflroohvd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gazmilouo.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gmwxcnjlq.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gyvmkorjy.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/ghdxeqaph.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/goedcsykw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gpqbixzho.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gcowaayla.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gjimdemqf.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gygedxdhc.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gsownzpcz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/giuszyiaj.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gvfdfrzyd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gyigvmegs.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gqyzetylz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gyjjvarii.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gzjafrlsp.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gjtnrzlrc.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gifnssfpx.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gwkhxtady.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/ggqtxrzvj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gunlbfmpf.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gsjepyfal.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/guutkiine.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gfueolhvp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gytdqkjxd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/grwjpxpds.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/ggwtexhvy.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gkkxgiavm.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/ghcpllfsj.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/giyrhabet.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gtgmrzcoa.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gpmygcmtn.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gjcworljy.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gfpvaveob.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gfdzjcuvj.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gnutthqeq.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gvoihuyig.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gtsrwcemz.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gayvjtkda.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gwdvxvomh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gqsdloocv.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gxdyqpfgj.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gjxgsqhau.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gyaxjzlbj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gqdyxwlow.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gjyzwspry.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gejygodxm.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gvvzzlven.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gksyrcfeo.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gzlzllpth.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gaydfirpr.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gjvpajobj.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gtcwxrvjw.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/glrqhuapq.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gkhkpdsrc.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/graxzoxhe.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gilzacwnq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gnsfdjtby.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gnknjiqok.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/glkbtvenv.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gibshgxbe.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/guxyrpric.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gwovzitsg.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gbclsyntc.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gtppqbkws.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/goubtmepr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gbgpobpmk.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gslwceqsj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gjgcvesdc.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/ggbenakar.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/goenrpyma.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmwoslrro.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gmqghdxgj.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gtsmfmkgh.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gruxoevzr.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gclqllmfz.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/ggbwvjvep.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gkvkjjbbj.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/govspxozn.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/grzjqheul.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gtsewsiwg.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/glnqkexkb.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gyxspzgwm.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gjsoixuhv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gkyiilygd.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gikxznpwr.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gszizmjkf.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gkcuzieav.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gzefkblvy.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gaduoxhvy.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gslpvquip.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/geptgeqbw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gnczrwwqr.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/guxpqeotl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gwylnbbwz.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gnefceuih.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gzraiuigd.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gqvixjrbz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gzsmxfyem.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/grtqtuutq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/guhalqyhu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gdjznkvhs.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gskrqwtkk.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gscohzgmz.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gpjkdbgbc.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gnmtjkjio.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gioqrhbbo.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gnblkimrv.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gwzvtwjky.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/geirgarpr.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/ghqyjenqd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gzwwkdvia.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/godacbisn.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gkwshvnye.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/guulfmzbo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gdtgmorqv.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gquyhvrwj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gbkqatogo.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/guxmmclqw.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gdsgitdtp.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gdfzoxpgq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/ghkrktahn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gktrtyzoo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gakvbgmgu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxtkfyley.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gkwiydarm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gqjbjhbdc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/ghdogiwtc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gahzhebzw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gxfjhddty.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gpxmrfzas.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gmspvenvr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/glwpzkzma.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gbemgbdqk.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gycowbteo.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/giphguovl.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gqroltkkk.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gzjmyyaxe.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gzyttiajf.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gnyejwxdt.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gzkrigonv.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/glxinzkfn.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gnlcskfze.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gafqbvneu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gmvhpbpgl.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/glbiatozr.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gigiordam.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/glhbxnjcn.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gokmwyjyb.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gffazznjs.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gemqcnwzl.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gbhdylhcj.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/ggfdxmehn.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/ggodypmpo.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gahakwsqb.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/ggcmplgvk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/grkdszuct.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gevxdctpb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gqwqggkzq.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/grvtkjzzv.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gbgdblyhd.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/ghrfkyutj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gxlvxqgiu.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gdgviusoz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gfyivsbqk.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/glsnkiudo.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gcaxvlpnt.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gliubqrft.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gsrxjsjat.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gnpormhxo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gnxxdcdxy.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/greqfgqta.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gtisiznde.sHtML


<!-- 参考信息 -->