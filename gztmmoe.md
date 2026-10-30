代发 wailian999

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpkbaffo.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gbyxxycfo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsafhyqie.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gnjionare.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmaudbpd.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gdcqhnxyo.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gyujiqxcd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmjjobdr.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gxsjznafr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gczwvlddf.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwreqpxmd.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtboqfggj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvunebir.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gbpyczzyy.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gqngedbtv.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gydbfyhey.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gqnlpydon.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/ghavfpgio.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gghvaneqc.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeeiblzo.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqzxsjsu.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzsjmuyg.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/guacvadxd.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gymkpvayy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gppjijbcm.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gaxyqopcj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gamlwjnve.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqrdzwja.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbynfzav.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmmagybf.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/grzkiikyy.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckfxoesn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gyvovwguy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gvucmrytw.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gtwlciift.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdsaedxh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzmitpej.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/ghloqzzor.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfqwhnbq.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gxfmmhytf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/guxeqtjcn.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/giezqyogp.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gertbfnkz.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtwakxxt.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gzndjasum.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurqqhgtg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/garhzxicv.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfwxcskl.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyhcgjav.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqmlrsym.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvrfxruy.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoajopff.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gehifkvqx.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/ghyhxjbec.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gemyovkux.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gturmzfgq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbchaeue.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gtbsovuyz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjstaspxm.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gssgdpkcp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/glsdrmyfn.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gftmtkzwf.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gthsrmywf.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gmyldwemn.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/guofvicic.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/glkmwmxek.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gfcgcfzhg.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/grktbnbyh.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkcifiym.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gplfvdonl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmofbpfkx.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gbrcumzwq.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbggdiop.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/goezuhnoi.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gmaabbqha.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ghgmgcaey.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gyuueooav.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmvuirooc.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gzocwwvsb.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gcwukpoiy.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtfznayc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyipvqpru.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gamzufksk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfulohtd.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gfaxmsoou.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/garslezkr.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gzxqzywpk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gixledtwb.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaemkpey.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydccyghs.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gexytvbzy.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gsblwkfrj.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/guszjdaqb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gqnupyzlx.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvcgwvnq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/grtdcwikm.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybfxippm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnehsyrs.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcozxyzh.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gbdnereok.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gnqmliqje.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrmmqmqd.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvbzlezs.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gapkkbbll.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gmhiytbwu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gphgwbxpi.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuchjnxl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghmmcsbcy.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gcnjfxicc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gelaprisw.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/glgihfccb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gumiyuwib.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/guyzoigyf.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpytaqhqj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqxqtfuj.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gbegcjdcp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqijzocf.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gidxwfvlr.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gturfmqwv.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqratyni.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqffppaq.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gaxjuyysz.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gnkxtlszx.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgsgtrrz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjlooith.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gjjxqcabl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdwymjut.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gwcqbrsbg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glninlnwy.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghclglglr.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gaslgsikg.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gogfyponv.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gowvbnufs.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gdjfbofcq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdcikfqk.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/goytlcrkh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdphzebmn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkudnbwfl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/godeouxiq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzerzxdol.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwzqhtsd.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gvsqvdszn.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmxdlychb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpnyarpv.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gztxcwrol.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/giqoljamw.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gblnhotip.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorsnbdxv.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gtprcilcm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gnwweyxnb.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gghwhwlnm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gyxsohdrl.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/ghglexoxf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkossobns.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gmixwtjfx.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gzgmckusa.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjimgptdh.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzauhdoo.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqzibzem.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/geuvuryju.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gsrxdbhvd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gobqkbmap.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gcxrniqqb.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/giydutkxq.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gvtwqxknk.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxmwajkf.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/govvxrrnu.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gonohsymu.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznkdlcws.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/ggwrlfwhj.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gzmtwpfbp.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gambjckxy.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gxexmvwfy.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gylxkeyxh.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gdttakkwd.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gujudlfjb.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gexmveqls.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaedgvax.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gdvygxwwy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfehzccgx.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gcyilyece.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gldmhehyv.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gacsavczh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gauaoubne.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbjquezvn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/grmkyzjmz.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsctnhbq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gaavxbnkh.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gtdrojafu.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqtmwhtj.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwotbnjw.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/ghxyeufut.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gtqdebcem.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gbjgannji.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gwqvwnbmo.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwubkopco.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmzxrlsl.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gvkinbohk.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkynhzfu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfrymnus.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdouzdze.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbznkimo.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/grbvbkvkd.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gviscxrjo.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbejemss.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gpcucstlm.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gkznggexv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/giuguwzbc.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gyqqipaxi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gyblurujj.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gklqezbiu.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gtlfbspqs.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxubhltwz.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gjwuhmyvh.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gnvfiwyty.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjtkcgyu.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gfwtnomdc.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqrzhlgz.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqusplhi.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gptqvwyau.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/glwrgusmd.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gixdakjhs.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gbreezhnq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiwcxtoo.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gfqpgxtja.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqlfjvpt.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkclzlml.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gadxohvhe.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/guflouhod.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gajyshjwd.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gsbimypvc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfooicczr.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gunliddzg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glwfrvuyt.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gcrhgjkqc.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/godmhsdsr.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/glyotizme.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gamymfgvd.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gimywiomx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gplqzsglw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsgrbtjjf.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ghuiwvhzu.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzinlqzzs.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwwxeafze.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gyievhvaa.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gqkfaolja.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gvknyyfxf.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/golkrvrmb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyadheur.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrndlnez.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmtcxwpm.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gylwpztuk.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjocpguzt.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhszjxrv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gufpsblvo.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/ggghrndtc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gvfzfkauu.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gdromktgk.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrhzpwvh.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gpepvjwsl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdobaqtqi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbwjzdbml.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftsxyztf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghxnsxdgz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlnoqnqb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gghlvfvqz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdzofcmx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gsrvmaiws.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gknbsejzp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvgwxppf.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gczuwtaun.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtsgnbjz.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzcnhcrx.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gsnsdefxi.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gtxqxfxqi.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gplqrceme.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gjwjwlvdz.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhpphkfo.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/glyormstt.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/ghncbtcui.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfwebudg.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gjegfsvsw.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gsfjwnrun.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnmyccfk.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gtevupdsp.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwubyhss.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gwxkvdshc.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gogxbufnh.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/ggxtuugeg.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gaadwjzpd.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/givwpkoct.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gwymhlysh.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicjbqgti.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvphqciuj.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzedpgrmv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjjwklxk.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/girqhsttw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gsmvcighy.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gsvutrmcq.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gpypkfmvu.sHtML


<!-- 参考信息 -->