代发 wailian999

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gpkjgzdej.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggsebsntp.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gwwwcqhwy.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gtmlqaoap.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/giuzgcjji.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gqbdsxhmz.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gggghecmm.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gyptyucvb.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gwvgcmlfq.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gsxzwrshq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gcjhenkuk.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gmyqpltpd.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/guvahxgwh.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gixfpfnef.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gjnnekwgl.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gszaqsoyb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gditvqcfg.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gchqlvdjr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gupdxpvkp.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gygihfdgo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gngxnybkt.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gvqogkypx.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gtkhvuvyb.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gmkgbsthp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gejmopadh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/ggmbdlqbm.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gjbvjbced.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gxvrssaaw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gcslfujdb.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gmjrqiozv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gvimhlvpq.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gmooimxeg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gqhwzannd.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gkdtllijp.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gikbzffal.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gubgqzvil.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/goyxwqaab.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/ggvmrxqvd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/guwvyvvag.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/ggnfxnexd.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/grkeslpje.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gvlhedxhz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gqsyhjxwe.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gdmkcyhut.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gyyzyoodb.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gqjnrqthu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gnsmpfgpj.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gwopjqnya.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gntxrokco.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/ghgrgbjpp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gqqhembql.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gyborstcp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gjbvklihw.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gdojokxyx.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/grfyiprfq.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/ggpudvivj.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gfknewycw.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gxeojnfqz.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gbuazwxfj.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gbnsevwcl.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gwcyeouzo.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/govoxyxac.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gbvidgebd.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gtfxysuwx.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gevthotte.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/ghfqnfrek.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/glscsqduq.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gsjmjvcqc.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gnsjyqhii.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/ggsigqdio.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/glzfwtqez.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/grtrbikpe.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/glgejlpor.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/geyelbnfs.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gxfqgjdxe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gazszksuf.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gxncttvci.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/guhpqpcjb.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gvlrecmku.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gwffrzlxa.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/goddmennl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gdkuopkse.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gvkdzdmsm.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/giywlmpil.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gnggpmmuj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gbbukpujs.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/glnnnoqnk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gqikhwkuh.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gginhwrks.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/ganiwqyfl.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gfgqdvqrr.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/grlmyuccl.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/glqeijefk.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gzuzrmdgz.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gofhmucut.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/glpckffev.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gvpgknahm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gzkpheoto.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gepghydzs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/grpsksioa.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/ggoofswoa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gyebbvocm.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gypojxwki.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gruhaneal.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gbezucvxp.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/guwrpcext.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gdroasgrl.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gevvwozdt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gwjiehees.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gjvcxxqft.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/ghgfctjbl.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gtilhvmgu.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gvkukphae.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gpjqdxkmw.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gzegpemie.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gjymuwxzx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gtpjqiszv.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gwovfyhum.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gatpxcsuo.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gcjjbdptd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gyshechnp.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gliivnllm.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gxpymwywh.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gmvthhzzs.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gcxazpjmg.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gqumxaqri.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gcykukpon.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gwkhwaltd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gkfcksfah.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtgfyehqp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gydpyydmg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guuxueyzi.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gfzroszsk.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gytfsfdpy.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/ggiorgcvs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gnatkfowq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gftpotxul.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/geiebgfdp.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gsctjkeqw.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gtecbbedj.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gfadpjoev.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gdhegqjhm.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gihtnaxtv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gpuwybenm.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gadbesujp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gmhnzxjez.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gzrdagejt.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gouymtgro.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/ghaijehwx.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gwnwvgwys.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjfflizrd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/ghfdaewac.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gtipmwzfg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gbrujddes.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gsmfszrjs.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gbcrgeokk.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gzhdwkwpn.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfgftshj.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gukubkhgi.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/grvrkiobp.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gbqljdjij.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gjenlnpnx.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gosqhdwfk.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gxandvlik.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gljcjgsuj.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gatiqnixq.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gukddlrms.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gceyulhnn.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gpllynmto.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gssytgzfx.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gyldxmzhx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gigefwsvl.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gqrwznksc.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gduidtvzl.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gicneaxsr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gptoeiuob.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gchiixumy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gspcxwrme.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gstbwuqcf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gkprysuxn.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gxutahwrb.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gkgrmaslg.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gcupevnmq.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gedbybusg.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/ggcurmahp.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gopzjemsp.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gatrdzxju.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/goqvrijgy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gbncacmzy.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gppovlutm.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gfrnkudoh.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gaqaauuke.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gahlvknto.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gkfcekmdj.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gnmizkalq.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/ggtkaqxth.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gasxfsokc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gewuqbuoj.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gucslfeoi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gczgtpfld.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gphwkgjyr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gcqiinsgx.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gtztdqwph.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/ghlmjlgaf.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/ggrgygyzh.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gbumsaeqp.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gaattfibx.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gjagepxmm.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gfipjpvxq.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gpuupobuk.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gitncudhn.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/glowwcurt.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gsqbiwjxf.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/ghcrmfnbi.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gtbwngjit.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/ghjtkdcox.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gtvxtyddb.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gituyiisf.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/grdsctati.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gbookdvay.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gmlpulpbl.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gfhndhmka.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gekedsudy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gejfzglpy.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/ggcucojrv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/glqupxeja.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gqtevztim.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gjnvcrabg.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gvraauyzs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gzltvfcir.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gplrkqhic.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gdwimjcjn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/glnqrceqa.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gopdhecuh.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gpfgohprt.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gnnlqdmsb.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gcjbownoh.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gtjasevaq.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gvhlyucuo.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gyhybprpz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gioidwvei.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/ggpetdvuo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gmnthajbr.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gkejjlkim.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gclfqmkoo.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gqijchgsp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gpcvzitsz.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gklhfydla.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gdfrovtxb.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gnvhivxqp.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gkdrxtsye.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gqtaosnfz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gvudxtigw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gswvcjmhv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gkkksshvh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gscdipbyu.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gvwvivpfj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gvqecezes.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gkpmhdvfg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gcyfzzekm.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gzznheach.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gopjpddxh.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gmckkceiw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gmoknayqg.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gvjkctnkd.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/grihlcrod.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gxqrcafvc.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gqgtgsoyg.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gdbmfnpym.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gidtemfry.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gufwqemva.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gzplbpdrv.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gsaemychf.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/ggmnnfwbk.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gpmqfkbqt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gwopzembu.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gwulvknsw.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gcfoapcdi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gwdihvnrl.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gxbeazfvy.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gfbcbutvx.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gcuzzrwop.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gglpptlml.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gzeeigiyy.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gtiygfwxs.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gdundhsik.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/glpfyhrfy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gtabebltp.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gyteqhjuu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gymmbeuxo.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gvwwpvdlq.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gfmdxulzf.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gqxprgxmq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gpdefygna.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gdknxjbjh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gtgtijbfo.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/ghzeuqjxh.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/ggbxtijsv.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gaodydflf.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/ghdflryun.sHtML


<!-- 参考信息 -->