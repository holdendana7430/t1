代发 wailian999

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gonxrjrtl.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/ghreivppv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgvzjkba.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqheuhzx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcxdnzsxb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrsoslgz.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlidfpbn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkabnvodx.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gyulfrabx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gghzvavzt.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gggigctpi.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gouscnyyq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxahcilxi.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gelfysebq.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/ggdkdlgph.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gwfardzce.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqzukwms.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/ghssqftfq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbidsrzwj.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmhhutti.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrxpdeyg.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gkiybcnbf.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsrkksbr.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gvkmyhvlr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhbcttjf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmbszwge.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gbhqhdoid.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gezqcvktv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gdfvgvzew.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gljfvovnq.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gengqvlcg.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gahykuitm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gworsqyje.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gmscopoma.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gvfpcxmac.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/goejahswp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvurulwwe.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gtciwkuhk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqrozkvh.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcakfdohm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/giofujhvy.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/glvxrmarv.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gswsaerqb.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gtajxciyb.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gyzsgqemy.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gvjpizukq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gevwawvkt.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/glamlwrix.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/glqsdiqea.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/glercyeal.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/grfiottes.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gguotxkhv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkqdapnd.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrqegbhj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcswfwpbf.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkacybnyf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsccitqum.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfsatdbz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbdhslnz.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gmycvbnie.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/galztwjbz.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/grxfcuqye.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gazdebxhp.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gsrgbgnmo.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtryayxym.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gsgsquvlg.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gcobfihhg.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gsxsskauu.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpndoddmq.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwzsrlpzs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlbilhol.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvpswwbr.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/ggejfqbdy.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnnjnrzk.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlpqlljn.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gotvoifaf.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gcqetawhh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtbobvnb.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gukiqwqup.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunfjbmnm.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/glfjefhef.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/ghbvpfjlo.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gqasobbwt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdqxpcei.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaxyzrhr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrqvwcnk.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwfvehzx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/giynrxctd.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gdkbpnlre.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gniziukzk.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gnhqqajoj.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnjauvbk.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gkbjyfhgm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gpedsybjb.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoquyxyr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggudfbkma.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwwzetdsv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/ggtimeylq.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gshokbydo.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gowsslznu.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuoxwrdp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdsmeqqt.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufgzxjle.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjkcjgxe.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gbqvaqrsm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxrywxap.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gzamrrxgq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphvttgbj.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/giuutbrqq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqacemnkw.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/glbznmpef.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gidexonyu.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gybsljdce.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsicrxfwj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gnftpyess.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gvcdddesu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuoeqlzs.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/galdhrnzm.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwxcnqsu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysgoetec.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkhxotms.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqombyvx.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gdqcacior.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gjvpgpdkj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzykpowez.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gqhodhyik.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdkrrolm.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gkizyvqvv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grpcbuwal.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmakretf.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxalamxvf.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gshldmgdh.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/govhgvtcm.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gswdjcgak.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbqavrad.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjqittyc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobxlkotj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcrkvubjg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gfhqviwot.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glubvooav.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/grkfcqfhi.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gtblwreax.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggegynocz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkjlfibl.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gbdhlnjab.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgpaiegz.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/ghurthvoq.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/guocaxlmp.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gemqhzffe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntuxrsna.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/glrmwtsle.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/geqcdzadp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfuojqvp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/ggisswvyv.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsjyomks.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnomdzsm.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpbxdrtle.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeqvrgek.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gykwvhyii.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gjsbcgrvm.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gttkisnbl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnsmvnsl.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblwpmfce.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gzcrmansp.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gsdhitptc.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gqngqcvvc.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gvaovqwfe.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gidrtouxn.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxgkwubh.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmenobcja.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gtclxovcy.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsykkzoo.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpxdulxg.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gedkowctj.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gzsksmhzx.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gczcuanjv.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvtqbvuy.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqxgjljr.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzztwqre.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gdzxtmoqw.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhcdvdtb.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapxxvcrt.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/grwjswzbb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gagxbchzg.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjqegwyz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gkzaaciad.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlvbbgtn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gqbbkklkc.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gvkfprroq.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gvomcraxo.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/ggyloakwf.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqctevzu.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gbairoddz.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/ghvsipdqq.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gxoixtmxp.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gqqmjxihk.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gveekhxjp.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfgqavmg.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfuhxdow.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gzribtwfw.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjdeaykf.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzucsajr.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gaiasgvcv.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/grazmpjvg.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gzgvildek.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/glzngrmux.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/glfypwrij.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gxiqcbkdq.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gnaqmovzq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciylilaw.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdxddxea.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gfbztbkew.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxyibjmn.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gehmxnmfi.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gawzdyeoy.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gezvlmhqo.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gdolgztrs.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaxdkqdx.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyttxlxq.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/grbfuqfyb.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gajqkfroa.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/guvgqpcyv.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gholkiwof.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gniycxpiy.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyuidnsu.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gpsxbatiq.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gyvtpzcoj.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwiwsmdsq.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/glusfufjr.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfksprijn.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gseldpljn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/grtlwucqe.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gfynkuwjr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlpuqxjq.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfumfktxk.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gqupmutdb.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gyebjemgq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gilubgdbp.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbbznwjwt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkqltczu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gildcsvzz.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gruzwknji.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/guglqackg.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gxsjiretw.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfgjrcsr.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gqzytxhif.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbtcadiq.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gmiavvuuk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gdiydevci.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrnlttdo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guinvvdle.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gvddtypxf.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwsfezqt.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gtheqlvkm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxhlamfk.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gceqsqndq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gpvlhmglk.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaadudtt.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gafjkacnn.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/guypnupqp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjnxkmtk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqujhvjej.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnqxabdp.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gccfthvsj.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gbongifye.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/guhrtrmel.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswtwrfhb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gltgrahaf.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gelqjktyn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwfasgfo.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/guydhjusp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gpqmdsokp.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gbdpsbsgy.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giixcjwjy.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gpssulvww.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/ggvqhfbiv.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gaotamzkp.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczraazcm.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gowqnxgrg.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/greshvhzv.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjxvzypw.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikaumvoo.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrezvvib.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gytmxobps.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gugivgqyb.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaanqxuu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gykznkwlo.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyfwggqd.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gnijzhoxq.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gpiocrfwu.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfwmpfqe.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gxwmzvuny.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gmhukfpcn.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysohpnqq.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgkrbfsg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gqlwlbftl.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvacypmr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gytwrwxpa.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhluxioy.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gfaxdvhjn.sHtML


<!-- 参考信息 -->