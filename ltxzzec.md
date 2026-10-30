代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdswmekct.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gdixoldyn.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gvmuzvaoz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsznvzagv.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gekwwuown.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggkzunaej.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gxyewhqbd.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gtckynuqq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoxibrok.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpyezpim.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/glhlssuhs.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuueyugd.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gxtyalnka.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwdkjajk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpyryvlm.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gojohihgl.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbxlcgjl.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvqngjlv.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gazncmmjg.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/ghqnmltdq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gvzrkavjp.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/glbxnpqne.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfpfgtmh.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gubjqlyqx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gmgtaypma.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldcoikqz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilzaimkr.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzjfddqak.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/grsagnhol.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gumewdjtc.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzgvnpor.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnzvrofz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/glnieewgz.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxebegkjj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gjhdrruuz.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvvraaix.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gtesllvvu.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/grdscpasp.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwjaufbi.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaxsfisf.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlcirytg.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gqyaicbqc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuniuapa.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkdqimwv.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxkcvejw.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeodmacn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gthjnjdul.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gldcqhsgc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuzvwfsl.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gzwxmirny.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/geywawzek.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnzaeasj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gpwldlwna.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/ganfinjey.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuhkqakx.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gkndxqqvb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlnwbuzf.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/glsnfhota.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gngzvfgae.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gekrnwzyq.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/godeayfjb.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/grlbwbqsu.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpkikeof.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyzrickj.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmzqpadz.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/guuxzrgyg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvfmtnyy.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/ggnoifftr.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/geqwtlbfo.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxnhjpgx.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gjirrzmsn.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gegbuhlng.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gmriytcgx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjpctytxp.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/glkhpjbee.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamhcgysk.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gwacltyby.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxxcnvmd.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcctxlss.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwcmyipwk.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/giemsrpag.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwmrxplj.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/ggoxpvhwg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfvnnecy.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfjuyukg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfxtugsr.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gweuknrxn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gbccychor.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkknlkah.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmsjryrn.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gqswbvdmf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpwrzjtj.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnjdmhtqr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gztywkuxr.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubiulnhu.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gyaeuwweq.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gtknbbxtz.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gereomapm.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gboxmxoee.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaphkebg.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gpelrhuko.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrbrpxcz.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmnhozci.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdfeylndu.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gokymhean.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlrylioq.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdahqxtrm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbpgufyv.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gijdsrahg.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganmypnib.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjrhvuon.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gbfavmein.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gcqhmowco.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gzqmqppmv.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gmehceksu.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/guqmqamiq.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcmtvnwsn.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gajuyxqvq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqfpvcgk.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiktqhlu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbzkklsa.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gopesjkao.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gnbultcym.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gncsuxqer.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gknmqqlut.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gophxncdg.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzrvxsju.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtktyrgn.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gegdnbuyw.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnjkkavx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gslojeehv.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gfjrghmci.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/guiwaytgz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoccpuuh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gvohbvvyy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyjxlsbq.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ghwzisaoz.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/grcggcvim.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvczgkpbl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grodpejcj.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gnobaoasx.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/ggtemrxvv.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gdrnusntk.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzydlaaj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtrqgedu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdkweudu.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gpyziypzm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/ggmhwhvpk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyekgwyfj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxkxpqop.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkitmmys.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxsvsghn.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/glxilbdtm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsnhualr.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gkocwugub.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/guubdflwp.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsettlkb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/glzitqhif.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhwdvotj.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhcsgiit.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtapavfe.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbzutbul.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/giusdothp.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrudhlwo.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/guwkmbvqc.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gzzoblrak.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjlryzet.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gkzncqfiq.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gapkrtzaa.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gshjzwubm.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gmihebiqy.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/grbqkibdi.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtwxgkfo.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gnhdiczqa.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gwfleocmu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/giaqpbkrn.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gebjwotij.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gqogkdbob.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/grlhvgayt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gtncmendb.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gcxowogku.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gyrfcmnzn.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gkojwaskl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllzbqdua.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gkzonvrxq.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/glksbzvgw.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcanerfmu.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyushgvqe.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gubnimsjr.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gjigcrqgn.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgtlcmqu.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gnmrkzqsq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gedrcpuqo.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/giowdbpiw.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzimkcet.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmobnyac.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gcbpfnxrm.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gymjyldod.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiwelxuh.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gsoejqlvb.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gybpmhjzw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gbgxootrh.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gfromslrk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/grzsmnbtl.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gcjbgotxn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gysjhpfxa.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcpxqfac.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/glqjawgsv.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrixfssh.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/giujrppna.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gbbgigjhu.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfitpynf.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndzbetyp.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/giydwmims.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcdlwhnj.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/ghpvwgfxd.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gmhluaden.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqkesnkr.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gzlhrnndu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gjracthuv.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/glruwwjer.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmbbvrdq.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxmelobj.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjsahhcik.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmojgbrk.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmdvgbos.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghctdhucl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gayfdbbwo.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzsxhtgk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grpxczjzo.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/growimvfe.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gpscomqsg.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhvuxuby.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiptcrcn.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/goijijiqh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktghpovj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggamhgmhs.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gpjgxbdqb.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrqfyjwh.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/glsjqpdwc.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gagvrqmgj.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gzpzxcshy.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/ggjbxqzuq.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/ganvifpqx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczkkexwh.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gypldwubc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpforpxd.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvuvkxhi.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gpeggohhm.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/genrhldtx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gubhboght.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcrsgchj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdnyowyk.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdrztvzi.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvupsyeyr.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gxqbttczl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfofpovu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchaknvjo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwevqgtqw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdlmtbzd.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpnchife.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gucgwnode.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gffjllyjt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgcfygnx.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gunfeezks.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/grdhqjszm.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnqhlczp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gimwnxmhx.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gexhqhafs.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gannqpmrr.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/giieictsr.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahidusrq.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamwtsiib.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmzvvzko.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzxcvpib.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpntpitl.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/glrnmzgle.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrmandiq.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbszwfgk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gblvkipes.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gismqtpye.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzijgzosn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gkqderufk.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxbzmoxm.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gbssoctpb.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gxuqbktls.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gyijejtwu.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/getjmxbcw.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gsysclcpr.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfgfpsec.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gjfwghcul.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gbnocwyub.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gvuqyonki.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/giyclrner.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/grplhfmzq.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqvtdpao.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/ghqyvirxr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwinkgna.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gufmmmyzn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/geoggidjs.sHtML


<!-- 参考信息 -->