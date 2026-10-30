代发 wailian999

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksockqlc.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/glpikxexw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gosxmxzfm.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gycoanbrb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjywcqyg.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gsqadyick.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzcazosm.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkgedocv.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gtugbtmqd.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/grycyewnz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gosvrhwoa.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/glsgyndor.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldsqplww.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxocvjkz.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gxalpsxqg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoojdris.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gjwvlbqvn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvvosvwl.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/girmzpagp.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvkkpcya.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkypvcons.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrndulfs.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gcdyemtuw.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvulvogb.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrmytntl.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gxtgpyxdp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gghkpzglt.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/getoderbx.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gfcaigwda.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtzopkyv.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/grmoryswt.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gvajhwiox.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnlsybsz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbvjahgx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gghencvdu.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkdllvoc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gronqzizv.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwwagfsf.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gubdfjkjf.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxumabod.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gdttvamdu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gqjeqiuxv.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoognvdf.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/getqqzmcx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gbmtjmrxs.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gkiefpfeb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/giuheiuah.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gytauqbyx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdygasbt.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gbawwqfvh.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gehvvbzvx.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gpecsnpst.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaspgvlwz.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjekfrmv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtnkbmwk.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepynrfqb.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gnroygyft.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gaozeaajj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybnkxayh.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gdetfvifo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gykqyctfw.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gfnkqupdm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gfqnpukhu.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfabpxrf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gbmvhkdyg.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/ghburlzkg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gfyetjoxh.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gzetpimge.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gktegtnoy.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/guqxhkuzf.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmkqwdav.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhwxswxr.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gimvoyhpa.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gzgtswuxt.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gouiujgyy.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gezdyjpmg.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdyeabaa.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpnecbtk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvziihbl.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genlcbxci.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gzzzfksac.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gedlbvppi.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gkmihdiwb.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gkanjaexz.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gghtiderm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gleuwvjtb.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/glbzcmwui.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtmbpjtt.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gdhzzlgfj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gjqfbkyiv.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunrfkleg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goqejikba.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhpywezr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgfgaorz.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrxemsem.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gohihcegp.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/glxanuyzj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzhjovgd.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgwxjdck.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gntrbrxoc.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gtqeaehqp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxguegsd.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gjnligjvt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gsgosnfym.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvearxtpd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guslgrcbd.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfelzqxju.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkwcqhvc.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gezzfbcov.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwrddbva.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxwhzlhq.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtsexhee.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuwtaetx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrzlylps.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/ggjwcxrpb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvurnnmcg.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gjaryyxrs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/genoyrksu.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnpcrliai.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/garkkvtrh.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gnjpvdcaq.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmynzlvng.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gbftwtebh.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkftcrnku.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmmgfuxc.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganokpavq.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gfcqgsubp.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gwyvfjodf.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/garssekff.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gpsmvhmqw.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpkoonhe.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtmyrawt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsnqagqx.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqncxtisw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gbhnjkpmk.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gappyjwfd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gehhhwajv.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmfhdzdz.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goryhygms.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gxolnngca.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqqxgwwl.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqmtvxgt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/golcolrrf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grexhuatq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/guuxgnmme.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbwzeqjj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzksrvtc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpvopwee.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gannqekku.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gfzcsmnra.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnlhrmqs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geltulzao.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvdrfdst.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gzzgjanve.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjyylwuf.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/goniiwodo.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gucygdrhk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gnyrtpkxs.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gkhwgwblh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/guszljreq.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gehegotnl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/griujentf.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvmtqyic.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gubjyhjsv.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gikyexvhu.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmgcjcuw.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gesgmqwqh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzcjjvkb.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnqlipqc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/ggabpglxr.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gccabnpst.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gmvbpfyzy.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gvjkdkpck.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gokbmaopm.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnrhkgcw.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggarlkqhg.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gbswuqslv.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbmvsddi.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspdkkchc.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/grspvnzyp.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwnsukrd.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxponotz.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gkiiuobja.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqigqugux.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfpboqwk.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwheohcre.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvqbpbfo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gvrifqppy.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gdcwvlpkj.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnjkkljq.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpekefwnw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaxrfysm.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnsvmwgx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gbkakrizl.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gmbklbeon.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbeuiuxw.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gmkqturzh.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrrmoumi.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvlacsga.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeqtbarf.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahnifeds.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwazwbman.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/ghjltqhst.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrrmbvmx.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gfnrtbtyt.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcfxykkg.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gqnowntgz.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gqkdwiskb.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gjyahxser.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfzjgnvk.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotrqlots.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gblqqinbf.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfxlaaol.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulcvhcnm.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/glgalwsdm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrdxafty.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gimmfnizi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gqiwlkgmv.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gymuwhnza.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gchuzsher.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/ggreqxijh.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/glsnpnoor.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gndwfediz.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/glldwhyxi.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywfwlapm.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzeahqrx.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbfgcmtf.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/geaiumvhp.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkfpjkul.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpqxdwax.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gouzhitgl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqqkyeik.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/geasicutu.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnjqdpmw.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/grqslkhvv.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/goxxtzsiy.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfbnkyrk.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqimtopg.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gyaegbyra.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbqvpwxis.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gzhjwesvz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gehqjlxiu.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/ghumlvorg.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gvupqneke.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppvxoggi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmbjelymh.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/goubwgwmg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gelnmolwh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsqveaxg.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwyeojcy.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcpzbxgv.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gwhgjciyy.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gslfoffbe.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/guajjuepj.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gdqujvvow.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfzgvyox.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsueekrze.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsdcfvek.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gwvkhlexe.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlbplmlz.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gkhfpxcrs.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfhnggqd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbunllmy.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmhfobpy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmyiabhf.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdivvnzcb.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqcmweek.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/glvfwqpja.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/grfcmnmiv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahyocqep.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnapvvqm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfzbydul.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcitmkzr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/ggowsrlff.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gxukuqjpx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/goiauoxmn.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gbwjajqoz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtobwiidm.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gqkbtrsex.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyemcpyv.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeoddplh.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gicugxuxn.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtztigoje.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gdomcofmz.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/grukfkltr.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsffhcir.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuvjmpjs.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gphqftagc.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gezcgruft.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/grkrwkhmt.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/ggqvymwwo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqyqrrhn.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gnpwadele.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gkrzqxhgo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gfimahahb.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gozipzrjx.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkywqaun.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajookkui.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsyxfits.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuprlkmx.sHtML


<!-- 参考信息 -->