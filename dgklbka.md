代发 wailian999

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gstqmnqfg.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gpwnhwtyx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gpiqigmmp.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gwtsjibrn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gwiyqoyam.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gyrlcxbwm.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gxyobsbrt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gseltyaju.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gnbayfcru.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnoegraxv.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gmqcxedln.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gzhxlgays.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gcrzsbqxv.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gyumndutr.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gwykrrefv.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gpwyezgpl.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gbqgvpjyo.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/guqdrqoch.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/grfbzwdgn.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/geoxnmiqi.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/ggniilgnp.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gjtunyvto.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gcaxfitum.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gbukhthwl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gjwtlkrey.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gathnjnhb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gfrwekqij.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gizehhwfb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/ghgnkadmj.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gduvbntgq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gcmrbnqoa.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/grnqkzuml.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gvyakwnal.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gugdlmxre.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gzrlfyinq.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gyxnhvzcw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/glguruzic.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/ggauzuygh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gubwuwgyu.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/glvjayupc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/giwatkbct.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gwatqzwiu.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gixqdmvat.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gtuflhddg.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gyjwwuhil.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gzmftuykk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gvdggkykd.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gbmmsrqsg.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gmvlpuyte.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gywqbrfmc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/getxnerly.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gbzvobfny.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gtoenhswo.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/greckrtxv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gjjclflvi.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gaiizbfzh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gvsbcbjkc.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gdfcqolec.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gqthlkjjg.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gwhejfddu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/ggkssynbm.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gspbpviun.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gzjsipcpl.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gmtzxlymz.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gravfkgyc.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gyramchxg.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gosmhwqgf.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gjtxjgwlp.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gvglopsqz.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gjikpzgmi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gcbjbmrrv.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gozrfypfg.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/guesydpkp.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/glymjypft.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/ghvlfhubw.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzklsefsz.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gunelcyfr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gaweqkrli.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gszcotiqq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gumohwgih.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gxstakbxp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gkiwikqas.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gvknriznc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/ggrngbjuq.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gmqusjwns.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gxjvrhgtc.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gjvxdynvq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/glugwwpkk.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gnaztrebu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gdszexrqj.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/guytoxivt.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gxsicpptx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gtgyrplfr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gxkyxiyjx.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gdetdiwnm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gwggiqnsd.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gnzsjbqvk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gqhmiidng.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gjfmfanjx.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gplpsrawb.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/ghfbwkpzy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gxompsjiq.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gxerxkkvd.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/geegsmfnf.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gwribygsl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gcnfqeaqh.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gpbvphvjo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/guunugrtn.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gaiwrgtay.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/ghfekzctr.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gdmiagvvz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gjjchytlo.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gqqytnndc.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gikkfoopd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/ghakqzrjv.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gvzowowdk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gishezpli.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gmzbpzoqx.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gfthgsxsi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gglfparsx.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gdytegyej.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gtconsqap.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gpovaujoh.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gvjvxqylw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gjjfnwvvv.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/guzufubsw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/govznjsff.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gdmbpbdym.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gxdsxqnrw.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/guzxydihh.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/ghkkufevj.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gefcofipj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/goyprowzt.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gkvpwfogb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gvqfgqzbo.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gcupohxjj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gpogonwpi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggpxbunrx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gjleohpar.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gignqdusy.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gymzyafpv.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/grkckspij.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/goujffvkr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gtoqnuimk.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gqcikhmyn.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gxvifvjdn.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gpdfgzhdf.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gbmvakcvo.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gqixhtbmj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gbknfgpcw.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/ggqiwgbet.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gpavyisgo.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gtunkyxfq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gfrynkhrv.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gqmrhcfdp.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gxzosruef.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gcrrpbfjt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/ginwoxgvt.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gbgescjpa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/giqpzonnk.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gvyzbyylh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gotmxtfjk.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gaewtvipy.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gwqjrczmn.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/giwbgwnjh.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/guaugycxt.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gftyqejtj.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gcdwyjfjg.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gnzohloig.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gyjyhlont.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/glhkhzbbo.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gftrgeywh.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gtephfugk.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gesldzddj.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gqdjbgbdy.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gbcwayblv.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gklmnoskn.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/giydbrosj.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gfwmymcpo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gkasvbvbi.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gzxiocfxc.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gbotimzmm.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/ggehwtygd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gkszjnruw.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gvkwhytkh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gewemzxor.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gfdgaentz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/ggngcksuk.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/ggawmaxrt.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gqzstkrug.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gkuoqnrhf.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gzzejtxav.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gfhjzmnxn.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/glnnbtztn.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gwzcnvsni.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gkmvgnhjq.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/grhhenavv.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gjvhumobj.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gfomyhxtt.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gjnzuzbrm.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gwjemgqei.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gejimnmaw.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/ggyspcvju.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gazzfqcxj.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gayczwoup.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gmxmcqnsv.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gwzfovbmr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gddvwoxlt.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gnxotnxaq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/grqrysnkm.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gafhgihkg.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gbrjlzimd.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gssbcjdye.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gqkmbodlv.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gotdlvsze.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gkilesyrt.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/goxcelnhl.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/goukjzglb.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gmuraezsm.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gvhpqkgoh.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gqjylebhf.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gzzlajbbu.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gziwqmibj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gdoaogffo.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gmimbhbrf.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gwoooepee.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gzadfkmij.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/grgunbpeg.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gdtcacseu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gzicnaznu.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gxzpnrwrq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gdpgdyeqg.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gwidocnwh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gmrshgess.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gtylvyfbx.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gdhtqvnwe.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gecxwbmso.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gxlfslduh.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gjgefqknm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gjhpllsmx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/glpdyafry.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/glblvnprm.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gbdaqelyi.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gzfhokrih.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/ggdfudsjv.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gigxbwniq.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gozyrwsbz.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gninhyree.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gplgixjgm.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gajctwynh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gzhevvgki.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gepzkkykr.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gktwqrfgf.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/ghicexvpd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gnumasnyx.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gjztqchuz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gyxtvhyii.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gwpwyqlqg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/galbzbhsm.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gorvjctgu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gjfeqgnfo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdjtvykrf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gloqonoaa.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaboucyvz.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gteytkknp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gkjyxzlac.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/grsxysguk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/ghpwyrzhe.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gvlhuhhzl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gpfwhtnov.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/ggwmpowbe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gepgwbvsp.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/ggorlejku.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gdanheeye.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gipllbyoj.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gorzawvdj.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gvhhyeuvq.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gwtkcbixa.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/goiyqcnum.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gveuxhwbe.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gncgxadao.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/ghrufklyf.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gosvkqoop.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gxdfkqylv.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gizhvovwb.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/glkoalrgt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/glysdijph.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gvaesjzov.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/glmcvenjm.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gmxaemwhw.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gdqnnynvz.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/guxgtqgvx.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gbctosqro.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gudqdupik.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gysithuqx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gygfzjzwo.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/guhujldzx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/guavqgzhf.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gayktfdet.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gugvqvdco.sHtML


<!-- 参考信息 -->