代发 wailian999

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gxwekldbs.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gizzxwpkg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gamnczmyb.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gaeodqrbc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gthmkjvgl.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gxogziiuk.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gstzeelso.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkilyejke.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gcpleqnzi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gotjybljr.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/ghyugrwhr.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/ggpnyfwvr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gdaopcygr.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gtxdlldmx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gwcraddny.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gsuddnzca.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gbiaosnem.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gllbwvghq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gppawjhyq.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gwvzthyfq.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gckexzmbq.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gitzqhuos.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gioizspcu.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gvmykzfll.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gbdyteocq.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gnvabxiwl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gqlelmkws.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gnnsbqiwr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gqvtxibzj.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gjshgkiut.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gvaqugesd.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gfmzxlxlc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gnmedzisr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gyccxwikz.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/glcfuvwuz.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/grcctphlj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gbkfwyhvu.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gwjkjebso.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gmpysbsgc.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/goypedahj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gzodtbtma.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gsnrjtiud.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gfhzrfskd.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gwxfpjzkf.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/glojwfqth.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gtabhywor.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gyqjijbrh.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gqhxeuvdi.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gezqmrjsy.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gfqukkwjm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/guzzecoea.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/grnagmsau.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gxwrdzblo.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/ggpzcwjfo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gysrqgjtz.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gyyfanqnl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gfkodijft.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gmympuapy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/grgqtwbfj.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/ggzeqccau.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gbisvphtf.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gcwsnfpyb.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gozmjfgak.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gdqlbtzyw.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/geufqorjv.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gtjpktahm.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gqezmaval.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gkelyigxs.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gsbeaipdz.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gjpsndjyd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/grynvfyod.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gcpwvbxdk.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gntcpnhsm.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/grcfthdvf.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/goiczjppx.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gemrqlryc.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gdmsygoja.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gyjuleekh.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gsqmyjtuh.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gwvvpcwhs.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gryihbcqg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gxlkrywos.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gaiaxdnkv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gixbjsror.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gezvrtsfc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gnsrrtgdh.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gazjysxuc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gyajftnmc.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/ghuwimlqb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/giffwjimp.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gzxznsjvs.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gqilkgmnu.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gsdffftch.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gnmxpyxxa.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/ggvzouogq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gvimqmssx.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gytdiqrag.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gsjmdhiuu.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gmrotbpwa.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gnybbazpk.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gepzhbtfz.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gsaycsxwi.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gkfrobyyn.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gvlpnmmei.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gvurmqwgg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/ggbroxzgw.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gyrzwmgoy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/ghyztmbbb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gemotatmh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gpsejsibj.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/glgkuagxy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/giikahczm.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gzmbcpphr.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gbvhkujft.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/ggexynavf.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gpljewkwf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gtszwikpg.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gulyziyxb.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gjvwdmtdr.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/giborkxmh.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gnbinecpj.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/grupurjnx.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gnqzawqci.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gpmwajupt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gxdxybyvu.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/glxmxotor.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gpdqavcva.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gyxfzmmhr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/guiwdjbjs.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/ggmcwltjx.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gsephyigm.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gcazdzjzm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gravgpzwu.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gplnvjyvm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gjhobbuzy.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/goynesaok.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gayxtjqiy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxnbtrcop.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gnceuybfz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcvnhoshe.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gxspgpoxi.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gpnnynnhm.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/ghtoxzvgc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gsoihkmyp.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gseidkxxg.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gtrweuizu.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/ghyfrbxve.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/glnqpmytd.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/ggdgiklkj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gciwubbgs.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gqzsdnibg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gdkkabfxk.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gxsznkamm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gmbnokclo.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gsiuwjlqy.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gxxjhvehy.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gnyewhprq.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gioszsbjg.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/glimqmqxf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gjisvvnjx.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gxemvjwdc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/goxgrhbkn.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/googveecm.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gfisvutxq.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/givixfyds.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gtdranqwz.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gwhzazban.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/giibwheki.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gwbuntjlh.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/godlvwypa.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gvtjuqhwz.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/ggronydnp.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gmswsjuum.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gjtqnnmjg.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/ggoqszsvs.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gobxrqdnn.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gkuuuqdff.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/ghfryrfry.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gdkudxoxc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gwwdipngw.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gbjsjxdml.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gxjczjtwq.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gkrjkkgfr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gvcvmsxfr.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gojmwfjui.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gunufwxfi.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gavmvowwi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gzuaeofwq.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gdttulqri.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gqavzytox.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/grdcorrjq.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gvptjzxot.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gfonmgpkm.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gjmpspzjn.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gdzonkjxu.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gqetgeowm.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gbiyxfgcu.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gdivoiszi.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gamvchqxs.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gbfvcjrco.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/glrsvaehk.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gzxgnzbdi.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gztqyuums.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gckdmapoi.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gfaudfohq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gytqrtuod.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/geysntatb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gqefhhtma.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gexcasmac.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gqyuaxrue.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/grvjbibcn.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gsgyscyez.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gjrzhrxkw.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gyqcetfkx.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gbwxxuota.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gzbdrzbzl.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gddanizfh.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/grfwjcica.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gvgxclhal.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gfocygvng.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gtifcdfwp.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/glbziuxdf.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/ggmiwpfce.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/glzwxomyz.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gwpgrrlxq.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gqrggwugz.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/goqbrccej.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gvkopfhoc.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gteknjtqg.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gzklekecl.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/grfcjxouo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gduemcmqq.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gwiceaspy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/ghfzkkwnb.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gfsztqhgw.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gdloqekmx.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gutavkbng.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gecvzpeih.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gfesuzqpm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gywluobmi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gyyhjpolz.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/gokzncqnb.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gawwhgdhh.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gbtreokjr.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/geeqwvzgs.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gcnuisqzc.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gyudtrvmq.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/guhtibouq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gjyfhrsdy.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/getqmzfsq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gfgwxfpxz.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/ggwvdsdil.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gmlnzlicy.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gjipxlxul.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/ghurkpkhl.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gcqlkixud.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gmusoshhz.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gnhwpcwpv.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/guimktvto.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gtxtoxvjp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/ggcmpuvtx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gedtrdtji.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/ggintivbg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gumkxofih.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gkcmaiayv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/ggojvehjv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gthvyphcg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gpfptjbyr.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gozqeqnvs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gubumcfec.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gwnjtpuiv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gxydsdnun.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gbpayijws.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gusnvilwv.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gfajwynsl.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gztmqhsbm.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gxmekeuep.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gbjrjdqre.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gvxcvztbj.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/geoktjbke.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gdgvzmmqe.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gdgrqpreg.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/glcydbdhw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gtzuktbwf.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gqcfkqsey.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmwtvbfq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/grginenyr.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gewcduykj.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gbytondud.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gwnmfvxkp.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gvptqthip.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gcuhuooax.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gmlxogpfm.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/grbejxbkz.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gscdenqus.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gzfdbmhdv.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gjkyfznwz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/giookqojt.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/ggtbiwdfb.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/ggbvapygb.sHtML


<!-- 参考信息 -->