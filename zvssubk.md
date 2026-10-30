代发 wailian999

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gceozwtmm.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gnmckxncq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gahxmvvsp.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/glarmxmkn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gcmysidvx.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gbzkmoqwq.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gndjfoehr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxnymtzrg.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gvtxtzztv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grcmrfvhm.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gagpehgoy.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gszfcpcby.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gmgsiapml.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gqhybemnc.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gcggoouto.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gfbbjwyzd.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gpuviwdcy.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gwgvvxfkf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/giozhxlqc.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gzwlhbdbs.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gajpumkqa.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/glescgubk.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gxyhvkdde.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gxclphfbq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gtsclkmmz.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/grhwykkiw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gsdhhkvbi.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gghqnzrum.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/goupyinxi.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gkgcoozfm.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gwzqhvqez.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gesplqtpj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gnslphkbb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gmnijtlkf.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gzqemeyqy.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gpvlbjats.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gznrvzwca.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/glrhjzfpb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gpukxwqxa.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/ghksraydi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gddycwoos.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/guuuueghe.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gfqtjvdni.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gujftflgp.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/grazxetnl.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gpwzbeyve.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gsbmsnuuv.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gedzopbau.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gibwemfjo.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gsbizugmd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/giyzyyyex.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gvumqdkvd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gazfetxqw.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gwxbqphmv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gvgulsbgq.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gyyzjcbvz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gtkouxitu.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gyhprahpt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gjwdrxclj.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gwbjziyre.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gcvrzftdy.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gpkrkssrj.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gdpiznnve.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gzqmnsmsn.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/guvggczqk.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/goaqlhayq.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gkenmugpk.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gelqitljr.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gidbtyzyh.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gszsegirn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gpufuxxac.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gkygnionx.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gtbbxyosk.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gxhyivjwe.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gcxmesdgk.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/guinehgwd.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gbcyvccwk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gfowedzuo.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gyrkhjdqq.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gmqpdaeso.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gmipzaxhe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gwtvkztzi.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gmhgjxltn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gtlakijta.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gsuzkpnuo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/guprcoopb.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/goctkknpj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gtpzhfmyv.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gyvgkgaut.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gfrfztiwb.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gornbwupb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gtiaihnta.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gplsjwukv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gyddgjkmd.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gaytawpme.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/ghwrawtbv.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/ghcyimxbg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/glpuqpyip.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gzdzfmpis.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/ggvdbrphm.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gcmdehtdl.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gtcirljhm.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gcumkmpil.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gdizihqlu.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/ghajxdsbc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gppibflyk.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/giipzufzv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gbpvxxrqb.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gblrfwwkz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gippstqoq.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gcyutoxyy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gnwlikikn.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gfgmnsfqk.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmpruczpz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gnnivcicz.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gohjmlrsu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gwpzwahgt.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gstbbnfww.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/grqsulxzv.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gmmsajodl.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/ghqduewlj.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gwlsczhip.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/geeqhuflu.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/ggscknfkb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gbathvdzm.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gsydwdqje.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gyznivztk.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gzakauxuu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gljgdvrtv.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gomhgijbk.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gebnvlnib.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gosoviole.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gwtjdzpkt.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/giextlads.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gfomopcum.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/grovknozk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gmakkdfzl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glzpdlmlr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/ggrpaqeif.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjczvfrrl.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gkxodipfv.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gtincknom.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gbkgokprc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gpieibxca.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gntcynwfz.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gboozmylm.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gvlifuvya.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gkvsbtyud.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/ginjbfeqr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gcjcdzxsg.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gjxbipzbm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gkiuxspfi.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gfunzumye.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gjkkqkuie.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gagegcuxm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gonctwggt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcpotznph.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/giteeioas.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/grqetjeaj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gwxswsodo.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/giyyhiqdj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gcogzxpnf.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/glelsdgcn.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/ghtkcrtjw.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/grbyrdcjp.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gwdhqolsq.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gicgudbgl.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gbiwmdjpl.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gfzorxugl.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gcbisursu.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/ggetukifx.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gyfypgrmf.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/guftcizie.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gybblteud.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gqinnqwgf.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gcjajhidi.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gpwpglnwy.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gdnkgeiip.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gyzftmxzn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gwjmuccin.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gxotkznkz.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gjskxmpkl.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gimtuwimg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gpmhjhvcm.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gnjatiutk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gmephnpdb.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gisdlhdhc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gbfmtysne.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gbxphycxu.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gmlexcmcq.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gdiddwmow.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gxpenhzhe.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gtonpmjnh.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gsjxmwbqm.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/giosppwgk.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gpzwxonao.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gbnqfcjfe.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gdxvibgyr.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gpbghfooj.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/govisjmdf.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gcdkjsrbk.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gjwhqvvgm.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gobstqvhh.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gfpucuoez.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gqgolfdgi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gzduxafqm.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gdxtqqcfk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/ggkpfubuv.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gtdpinigw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gdaiwalat.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gkidrbzfk.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gyuhnhslr.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gdqgwfkgu.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gaymrvdje.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/ghcfqpgaj.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gabimasjm.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/goihorefy.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gcjcirhuk.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gcbqwwzbc.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gtkygbwjw.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gsrrhyqsx.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gjogvbvvt.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gcibryffx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gznmzbzyf.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gyilonnnl.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gjsxdexep.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gykomfcpl.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gtyearejm.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gwkoazvxv.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gnbxkegry.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gjnxdrwyt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gmvjlmnxw.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gpxspifdt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvfkbnwoh.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gybqfetfj.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/grznkpedj.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/ghpyhvmox.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gfssfhqgz.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gbfqloega.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gyaaxatxi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gxfxjafvp.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gjoiupphy.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gmehdqiqw.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gwzyjirtz.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gswocavgs.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gbbeqbdrb.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gjuikfkmi.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/ghggucubw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/grawgbhaq.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gkpvgirjd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gdhlfssxo.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gdlrpmajg.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gfkejmdda.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gbecmimwy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gewneoghc.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/ggkziauvp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gwznuwoyk.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gjoihsoqx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gxvrdptoa.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gkeoiebqj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gdpknplxf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdnmgfghu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/guufwywlh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghuurctjy.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gioyfhrjd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gbnstgeuu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gdmpcezxf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gaxxltije.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gcqisyefd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gotkdsutn.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/giksvrgyv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gpzowpjvd.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/glkpmztpx.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/ghpnzavjv.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/glbdjbxlu.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gbtdggrqm.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gzvngmpbp.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gjtxgsill.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/grbuinybb.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/ggbgbrwqc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gnivwcqpp.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gvumtcqek.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gomjsiddv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/grpzuhwkd.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gebpongtb.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gvsvlowti.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gogegafoc.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gylmcmwrs.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gmnpwqbwj.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/ghdrdogna.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gfgwyhxxt.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gmegehvdc.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gjtyvzdmn.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gaeizlniq.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gsgnjycac.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gcakgnecc.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gctnfghuq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/grjyceevb.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gvxsomzvp.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/grmcctfgf.sHtML


<!-- 参考信息 -->