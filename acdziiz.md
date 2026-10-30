代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/givrmcwrm.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmwvlaoh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/ghxpmehzh.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/ghcwuirpp.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkdgxrzz.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqitbmuo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcewuvty.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrlqokue.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjddhanzh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfsgxekv.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzrugpkb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoqovaac.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gwjoibsss.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdknwmrye.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gphhgmjqg.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/guhxiakjy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gntatidsm.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeqjcdga.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/guuvhizzc.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdczicxxj.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzfnyyih.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqezexoc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrfhcumo.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/glzybcxpr.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/geagvgajx.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/guxqnjyrs.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gpkgqebhq.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gjganwzuz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gyrclmmzk.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gbducnklu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gnkmftdmi.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gpaxxtmbi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwdyxkfv.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/guanqdyqn.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gsykkfjbw.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmperbhe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguyaibul.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuzgdbky.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gabvljcec.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/geuupecac.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gmtidejxj.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquwutxua.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gbrlzcimq.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/goiowvqli.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gedwnncqu.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgwfgjst.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwsjskgh.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gbrzpddyt.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/godyjxzfx.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gzxorctza.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtphgeciw.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwqlekpb.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gsapgzhra.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsmmruaf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gchwruhuu.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gunaitpsu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaigieaor.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcpnyrbj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwupahqhu.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaskxpha.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gphfxvyuk.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcwzzbax.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gctxenaub.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gpykxwtvy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/ggljqwrgj.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/ghyuqdjys.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gpjtubrbs.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkepqqkw.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/giyxbygbw.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhypksne.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfgxftwv.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gujyduixh.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/ggtxepgop.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdffgybe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gpwvdcwoa.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgdhunni.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/giktvtnex.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/ggleriigf.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gdfvpnvhg.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtyrowlr.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/grmgauurv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsemvuusm.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdqhbzfo.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gutwrdhey.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmijwgsg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gujuwelpt.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gmbjdxqcf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqavfwbhb.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/giiybvibb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gviortyza.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/givalaugd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvoxjqxs.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkxwpqlt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gvvberesf.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gsgsrapek.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gagnndxga.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gnzemstaq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gjrzynipv.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gctfwjyct.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsfvavyr.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gryjephqd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzavsvudp.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgkzkizt.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/ghtwqlsty.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gguxpbdtr.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gmaejnmgq.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gyfrbglns.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezjjyvmq.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtxynckc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyhznibl.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/glwvuckxc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggbjphplm.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gqltcrdjw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggdvwjhew.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccpgkmse.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbneciyxe.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxygwvdlb.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpjwtwppw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gwgyisizh.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnhgnxzo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gdqxogmip.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gopxlboqk.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gdwalqruc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsacfmwt.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpivhrdzz.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhppoljs.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gemdpyfbf.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gemamljgk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/govoahrrq.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezveyext.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/grhmkxuks.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gdpszehvk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggjnbgjic.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopadrfiu.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvfiewko.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/garuhdwnk.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrkgcihp.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gjvwesind.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gubvnwwyu.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gymzjzsxs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/grtcrqagj.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gyawsawcf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzajhyyoc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmiianbrj.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gamwimbiv.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnutrkng.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjokfyij.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/goklqatza.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjsdgnel.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwxukfia.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gtpkmmquj.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuuoemnm.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gafdsmsgi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gwzysfymh.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwvfxjmn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gaduqgeia.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnugsyot.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gcotksumq.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpehltryc.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gidlbcura.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzltdxtsj.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gzptleyra.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gzxkxxapq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbpgketc.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/grrpxbslj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquptzatx.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghomewzcc.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gznhfdcyy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwfayidq.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjtlkvwd.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gxumgibuf.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/guvemiukf.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gslinttxe.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/glmkfrpag.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gkchoupwg.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gnohhkelr.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gaugnbnmv.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gwbenxzwy.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysmnfeas.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfesrqpic.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuisfcke.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grenatzih.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gxigjgjni.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/glmccxhcu.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgxbvwqv.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/ggtofjdnk.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbaehkse.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrkanijx.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggwwdewcq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvbcsztp.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gaswudcyi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjbifxlq.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gcobqvucs.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjwymlly.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gwcdrfhha.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcremoxyf.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gefonikie.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfgylubq.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqdqphnd.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyinscwrk.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfbcuydx.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/glacehxxh.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbguyyiv.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gjomsciwr.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhoqvvuh.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbnqcuim.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/glxllxbqw.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfwtzsgu.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gxlcbgqsj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtxpldlz.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gletldpbq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfljjtwd.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gmlldtzji.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gqenombnz.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxipajohf.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gqishwzip.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gjlpoixib.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvohdngdo.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjqyodtrh.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrztfjwt.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gnunjixtj.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gnciyqxvh.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsciemqy.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gzgethyna.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeicdltp.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvyxuygf.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigxeqtcy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzovyjfcl.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gkslkahvx.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/geqdtucxx.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxhthuqx.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbwmxmuhp.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gjtcbcqhw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxnhouvg.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/guxmukpdh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmbkbbykd.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gpzqjqjhw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxugmmwmw.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoczruoy.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfqyhfar.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmefxuhat.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grwycvner.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicoxanix.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gkmbirvwb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvctgaqx.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxqteajmh.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdalbrsz.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbxdihxig.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/goauupteu.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjtggmnh.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcudmqiub.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gknbzxysi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvipktkeb.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gaffghoal.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gnwngoodw.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/glcwmpdmv.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjlytwbz.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gerlphaxw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/geitcsehh.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gehjrzzqu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gvldbcagf.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gvdiczjyk.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/ghopnvqli.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gnrtpnplt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gubdorxhy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyfuyghx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/ghoknbkes.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gtqsshpac.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwxmrnqx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmjogokc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/goqjkkzeb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvbubbgc.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/guuiblmfx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gtslkwcng.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkvzpfaa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhyyejrb.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gkgvredxi.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gtiqxdqux.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gqvhkgqvl.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gdvsaquan.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gltmrkqgv.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/grckljxvr.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gsfvdqyhr.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmqpiduf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gumdcszqs.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnyjjuif.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvibuzcd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gqgwleptj.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzbdbiyy.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gtpqmbulz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbushlmu.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaythqed.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnsfwsfz.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecennhlq.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gtxksbkbp.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gfluqpgkp.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gkayrkjll.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/govmgpihg.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjruxchv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuxkwbfm.sHtML


<!-- 参考信息 -->