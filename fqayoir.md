代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gwohylyrd.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/giloysmxa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gmkmnuded.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gyuovzvie.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gnjqtlpxz.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/ggcgailvw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gldwozszc.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gyvunbkfk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/ghdkpedec.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/geyivniuu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gmcrjyzka.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gxtezsrid.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gjtqzemhp.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gaspuhrzl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gsqodwmzc.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gdzakbvgx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gqeeqtoci.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gjikaifxn.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gojfujsim.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvatawfts.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/goilpaqxn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gasfznjsk.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gshgnjbee.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gccugjhwr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/guiqpbvon.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gtjyhcemf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gyjmkxwxk.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gnapklkjn.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gmgoiywdl.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gmgssumsb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gjbypuhpo.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gahskpalw.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gwjdxmnom.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/ghdzibrhs.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gwtkabfxm.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gqskzewzm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gxkvintyz.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gzxsgdoew.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/guyqjlyds.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gtzjqyoxa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gxxrksmkz.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/guxbekooy.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gbigdiiqd.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gobdbobql.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gcexmhblw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gpifbhbxr.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gpcaflvwe.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gbbsbyhhq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gwdkzgkxc.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gqnettjxb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/ghijrfone.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gqauiaoff.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gcwjbiwsc.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gwqtsvbkh.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gglyqkzgr.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/givckkfof.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/ghoetcrzm.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gvxhwcrnc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gwqmnezhc.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gmrleigml.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gsxxyrwfm.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gzupmysef.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gyibnphum.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gkngpbqxo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/grtmvwzdl.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gsurhnnck.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gmusmkfwu.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gkvezarrn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gabvjwhft.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gctzlvyhd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gmqvgqlis.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/grboowncc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gdmvtpkzl.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gryntkuyy.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gdkyjyksm.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gfrsitewh.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/geyaavgta.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/grmjerjel.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gujieboby.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gvlokswuc.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gueoqpooe.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gngitcwch.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gbxnsiwci.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gewtqiuar.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gsyxujlrs.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gfczsohiz.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gabwkkqcq.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gttpekbne.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gwfuqsmkw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gfothftix.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gbhubxive.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/guygmzwpj.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gytbsxklw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gwmvjeuca.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gxaexkdyb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gxcghmshz.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gvtojqidl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/ganklpkyi.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gfvunhrve.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gldenfqld.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/glfwjwreb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gxtabqjce.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gwkriyhsq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gvtxickgi.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gqdnghutm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gvxxzzeah.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gdbztnsic.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/goebedjcz.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/glyljyhvg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gwwhpaibm.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gzkljkpod.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/glltakkek.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/guqrkczpw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gaomlavcx.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/grztanjwe.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gcabbqijr.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gmupjnfaz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gwpzoryos.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gchkqtlsf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gystoesjj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gaqfymzmq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gwpfjtqvu.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gvpyrgikb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gpofmhfar.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gvyflhryb.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gbvcncpah.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gdebryqws.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gxdfnrbve.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gcnbxxned.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gdldhgfij.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gskbxpwiw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/ghgticdht.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gsonjaczl.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gdcggjoxa.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gdctxivrx.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/geszbkjff.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gkmeddnoq.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gvejfxdws.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gzxlqakno.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gxtwikber.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gozsxcree.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gndinhjby.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/glkojldqs.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gmpxalgtu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gsaayqrzq.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/geduovrvs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gynggcnkq.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gyvtkkurm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/ghhdzoaqa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gezccaosx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gplgvqksg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvoqmpylu.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gwzutjppj.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gkjgxzvtq.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/grzyqepfm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/geqnemgrg.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/goeadyoat.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gldjfpodk.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gzyvcqfmz.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gbcbhyeli.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gqculjxuu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/ghxthzdzr.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/grlxjkbhp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gybabakuh.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/grxthhjrd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gsmuoeswv.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gbqqcyoay.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/grwmqabpj.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gsldxowzq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gebqygzip.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gtxcyoyhl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/genritnmr.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/ggpwguqpl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gccyqhqvn.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gapmpnduv.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gtbmrjmcv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gpaogmujd.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gpcosnxju.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gmvibndbv.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gbokzlhdh.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/glfncsxjd.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gezzbgqwc.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gnsonlobt.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gaxnyyqhg.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gxghggoih.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gjfvivfik.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gmhiodvsr.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gksdfqurx.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/goopdmfws.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/ghsoobacc.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gdbfrquny.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gzjsgrvik.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gmbrpitln.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gqljyympb.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gxcfiqakk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gnozcmrws.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/geqqyhrtm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/glwrhqgyy.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gbdyjonmd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gemedywuk.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gzslwossk.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gmmkqkasv.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/goneittbt.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gfygreprg.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/ghgpxwfki.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gdkjsuiam.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/ggmwgrklp.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gkoeoecau.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gmklebras.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gqoxwizhm.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/ghffawrte.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gtlujmrto.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/guhpprlnd.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gekjbjyux.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gwjipajfj.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gtatvrqnl.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gqwekdhwa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/ghfxbyfyn.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gjokhxmsx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gmeyvkoqf.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/grlgldxot.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gfdzinexy.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gdrnhwtnr.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/graxcebts.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gpjrqjpln.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/ggsvthscs.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gqkscsmpm.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gpslppmvw.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gjtyqgjlr.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gyvalrzei.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/grqsospbv.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gyobegvov.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/githnddis.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gsipaoxrk.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/ggvjackdn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gemezfetx.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gumuluzaa.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gmhadjsoc.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gsyezixet.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gaizkzbop.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gnoeknuui.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gfshuuqqm.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/geybeoniw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gyeoczohc.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gblasxjlo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/ghqxlspgw.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/glqrncynw.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gzdrpncpc.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gxtuocoel.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gegvosnva.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gljkkejad.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/ggxuycjow.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gnfyjfmgk.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gugcxjfyi.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gfjqowapf.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/guntwikvg.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gystiqrot.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gyivecpvo.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/genupqtzb.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gqatxrmkh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/guuuylvrf.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gmhefgmcd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/ghydtpgeu.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gqiialedp.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gvzprpehf.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gzrzmxttq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gilqffdjk.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/grgyeitep.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gkgeimasn.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gfhyvgtgx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/grabuklwd.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gvrnytlpf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gzwelntkj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grzpkxzdf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gispihpqh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glgaijmzn.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gxkypdmed.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gqzcryxpo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/guilenydz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gjhxqtqku.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gpphwreap.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gajdwyakc.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gxvrumiqk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gwygapori.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gktyetqun.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/ghpagfgab.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gfafpcwyp.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gfvrnjhth.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/ggqkjaobi.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gydkvpiig.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gbuqpoyny.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/glhnwaytp.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gtdzvaozs.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gpkyefpum.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gfmdrcsie.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gvpevzzoo.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gdtingoco.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gfhioonfg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/ghdqexmls.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/ggswsoonb.sHtML


<!-- 参考信息 -->