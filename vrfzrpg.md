代发 wailian999

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gwbozimkc.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/giifdwkrv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwcidzxg.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/glannqdtq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbwlmgyb.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcielcqfm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhapvrtv.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhxzqcda.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gniyshncg.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqejhbxxs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvxmghvxv.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gugzcxttz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/germcjork.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyybzpyno.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gekxhmcag.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobibuozm.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcaotqug.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/geobphloj.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gtxjymffi.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gakhubysg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/grkqemgvg.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gnjfvqvtj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsavhxnxv.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxxeflfb.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golfvoccq.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gjxnfyksi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gcesfypzj.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbdtqtcf.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/guiittdez.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgepfutn.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfttmaah.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gurzxfzbj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gvixxsyju.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gmgjwhzdt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gzoernmno.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaheyrpra.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gqgbrxqbo.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykbetqqx.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gdhtlcfve.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrlsppnc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gxjoilrcp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdunkfbm.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiihyczi.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsajvxjcs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxwvnogw.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gmbelqosi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/groozjllb.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guymjkqhw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gzwxutcaq.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/glqncuast.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxsuryox.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gmlggsuqm.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkzcmxxj.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gywjtadte.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gnmiyhyca.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/guicjbdvt.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfheahpa.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ghilltpvv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzyednmi.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejkzkyzr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmathakg.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/glnpcjkjb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gubpqzocw.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/goavkjodo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvboyrkxd.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gojvkozct.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujrexlxm.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gvojekgpv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqllcyxc.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhtzypyy.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkidofpb.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/guzloapgg.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbszkjcag.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gvrfykjpr.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwngjxved.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblhasrhx.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwctamkam.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvhgbdpn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gmmwwulhb.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbxkanyx.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcuikdhk.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gkckbqzid.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gznhxayol.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddzrvduo.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvxymlrz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcsrjbga.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ghilnhvtn.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/glonoefpc.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gkqsgfhqw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwzpztmc.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gqmuruczi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqciusru.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gozuxirvo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgnblmbv.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/ghucldegz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gkhcabvdo.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gannjfymc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllkpujal.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfoqdttct.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpbwjwlm.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gztxdlzmz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/guxnnegdv.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gkvfsrqvs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gqhmtnylx.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlbnkrug.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufjszllx.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gponwbfky.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gvfdgeusd.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxxzjzin.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/grhsrxfcn.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gbscxkrkj.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibcwihib.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuhpwgoc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gvepibgfd.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/ghphaawwe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggxntzint.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gupdoqnaj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmjbalwx.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdbvwzqik.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gimhkkfkk.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrptsrit.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnypmesck.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrnabhyl.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwpcamxk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwupnersf.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/glzrreywt.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/ggvgjehps.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gkknovhds.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gguejejyi.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gudbbyzbh.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gagpmtdwv.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/glsagpdmy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gabbfwakh.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gyetyqtsk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/goifcncyl.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrtffjec.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giexztreq.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gwzsboryk.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ghqeljpcq.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzcexnfp.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogfyniuu.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gseosbagm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gexddlkyy.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/geqamkpgb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwbysoxe.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjosrgbq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnrxmnmq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztyyezyq.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrirnpii.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwefjbva.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gkrbpvvgm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gizdwqbde.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/grdwyhsgs.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfamkbipo.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmpvmdim.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/ggahdqcuy.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gzmwcuwvj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gvnzzkbol.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gsunzjwfn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdclolzol.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gvecgraal.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkktagqkh.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gjhusbcyr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpohzfirc.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjjmlqco.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gdojhbidn.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gtjtovzxd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gahndxqqf.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gtrqfounv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/grvxbxzpu.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gpikgjidd.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkquyupc.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gapjgoenl.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/glrfxofta.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiuchhmy.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/govqvkahl.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gsjphhtjl.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gzcqkuvpb.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gsptfsfrd.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gzkegmnbz.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/grjpoetjv.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gpvuztdat.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/guezpolza.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gqcxmilcl.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gewnvxqgs.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gebbvnbca.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgtcfvwi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gwsrctzys.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/grtingqwj.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gscaqidrs.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvmznffe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gknzjgbqa.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhdizlmh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gslpejsrn.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gdjcjszlv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guullgyob.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvljqxbzv.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwqoteos.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnsecavk.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgbwlkic.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gpzadkrcy.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdhpegfy.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gsumllbcj.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gmiggsvkg.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoejvchf.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gcnjzxluz.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcvmagcg.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmmhmrtv.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gpgxmtpcm.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaolujmm.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnazxdrn.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkxwlvir.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/grufkyycv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecyqptzb.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/glmfnyccr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/ghnwinlwh.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gahysvbtd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpumgdpn.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/grnpjttfr.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/ghekgwixl.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/geytrfxqw.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxpvgzjo.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdidqyarc.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gsdurqrvn.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gqzawxrso.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gjkqhotos.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtdfdpph.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gizrfxjyw.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gibepwulx.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfxvtugu.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdsjobxm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grokycbco.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gvikpsiuc.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gujdaridk.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gbbyafxwd.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gopwdabol.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/ggtwhcael.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzqutlob.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/genhelzdx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghjhiddwy.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gobkovyuz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzuxtsvu.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gptweefjs.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gppesfyto.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gutguotsu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbesbdfdv.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsegehjpp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gbhawecnr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnnqakgr.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfwexmtfc.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvukciwu.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/glygnioac.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/goginterd.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gpwtdjwiq.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gwqswhzuu.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/ghgogxbzg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gmovvcqvv.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gqrfzbwnn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gientmbng.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpbnuhgl.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/geqhgdgtz.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuefjfqh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbwwnxhb.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpmbdmus.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gglfyhlru.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gmzfpnrnh.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/glfxgaitg.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsgaufbl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gvootjytu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbybrzufz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqoicaor.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhcevijx.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gldqvrait.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/ggihzlsat.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjkonqqh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxlzuxad.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcjmilgr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gbzcyvszf.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzieqirg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuaumodl.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyobvqbg.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwslqipe.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gaimvxsje.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmdjyqsj.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gfclafwuy.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcligakx.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gknlcfspk.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfnmfvxz.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gsghwnrxc.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvjjuwiy.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkltlqtx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfjybdqw.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gtuzonqav.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goquadmbx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gshqtfeio.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glelexiwl.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gyrvsltzb.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gumducrit.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlsqemzo.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdreakawr.sHtML


<!-- 参考信息 -->