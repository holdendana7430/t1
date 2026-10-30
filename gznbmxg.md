代发 wailian999

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gnspdjlmy.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrcpbftt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxwihfod.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiiwgamh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpysvrlb.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfmssoen.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gdneosbeh.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grlyoqbtq.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuexpovv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnujbtnf.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwzwzylb.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxjcshwc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaechrdfj.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gcjvqpfik.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/giwuwtgvm.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbeourmq.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gejoeyqor.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gnhoztezh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqlbijwt.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvcyovir.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxjzanhl.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfxkeuho.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gepmotupl.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/grsjjdmvz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxqdunnl.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gwglqiqiw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/ghuhnyctg.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gtajrukqz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyjvkmkb.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gpregtmib.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gsforojtz.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gochuwlnf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gffumowcz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghamurtjg.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gxdbhrxzb.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gydphpxzd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gabctlnds.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gszsjpljk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gpowruvwk.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgpligqx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcbdghxo.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiekcsks.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gldtwqnbw.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvfkxrpy.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyxfhjge.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsirrtzvx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhfnsqeu.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gcxmiydin.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbomwgmme.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzzskocm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsthhmqgc.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnbotniv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gznuqgydk.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/ggraovamf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/golxcfiha.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/grwzlmcwy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/ghdshnngg.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbdyssng.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrkyerri.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gmioacyab.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gylisywch.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gekjskbly.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcyvbtup.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgznxcbh.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnkqkkji.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyyeowxx.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goartxqxs.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfpdwtqq.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gubbavobp.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gunmbuaou.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/guodrnlyj.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoisotzj.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiouovmi.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gmbrtdfgz.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gzoxdujyg.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtaoqhav.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gzdsawoqr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goynaqwzj.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhicckpv.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gycczkvnm.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gdgttrmft.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gtxwpyjma.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/genimrzfv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxgrtalf.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gruupboqc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiszcnmt.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxfagduz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcesfxcrg.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtzugokj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqrzmjri.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhmrnfzw.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gaajtnyiw.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gtjmsogsj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gssboeguq.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gffkvxfon.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsgjglky.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/geaqvwsve.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gjfrnjgxr.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwfacllqt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggefsriej.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnalyqda.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gjwbkvivb.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gvndfkpzv.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghyjrwuic.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcvkbqcn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gqugzomhw.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gankzxcfq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyxexgea.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuebttad.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyxeqwwdm.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grygqqyno.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/guorogvwf.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gixhratdc.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gitdyyvkc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gcypajlgd.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gpjvgufyb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgcmaamc.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfowzoywc.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gmikiqcsz.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/glhekfjqr.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gioacnhks.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfrqfxby.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gafofussn.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gxkmsdqxr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gkacyjcgb.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/ggkllvzbs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnzrbwqh.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslhrknik.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghilpkhif.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/grkamvldj.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/goowukkvt.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gestvdwto.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpjyqwic.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gpslhfgnz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gjhtirajp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmfdhcmk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gabloxbon.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqhugtfu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gaglsclgv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubuwyljt.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrwfghxg.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gypsrsvqh.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gedopfioy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/guoacfejg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsgpvywg.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzrqdrqf.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gexupfxxo.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gumjyascz.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/grhixynop.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsoxhdis.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoupfwos.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gegfmhdim.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gvwtqthsf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gjdhnbeff.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gndtmnrps.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfdsvtkr.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjxtyswct.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkfhaytu.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggymyzpun.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnxrqaju.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gownrdqiy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghukcyvem.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gfjaxqfio.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpgxisct.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiyxvomj.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gybzovkpv.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gcmqqvctu.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/glcnqgpqo.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gutigmeeb.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/govlifkih.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gnxgqipsw.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gocmoliqv.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklwtlsmf.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gljvhsgom.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/goqimpjpf.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gdcipgkmb.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorosscav.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfolvijy.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuahoxas.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gxviatzlg.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gpbjjldsj.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvircgaor.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlkzbmgf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gusxvsrev.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtsyqvoaj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gixxpmuce.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxaelwzk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gsuispizp.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gjandniao.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwoxozie.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gidgcpesi.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvyzlzig.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcgkektw.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyquclhl.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/ghyqrwkjt.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvbklqip.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gkknpqvuu.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gimbioxbb.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gykqaxjye.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gvkfldrdl.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gxajunxtm.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvnarzyv.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gzibdljfp.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmxutxtr.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnszzvnuu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxosguxls.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfilsscd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxopzheft.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkjvubae.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrqmvxhk.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gctislexj.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/ggodmmhgo.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gddxrbzyj.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gsfcjbghp.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzipisceb.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gdierthza.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuyqpgrx.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gpntvxbyn.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gmnhabzry.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqzqhiad.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqgfalypa.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gqqeqlzxn.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gigaqsowv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfqkgjtc.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwfxzbzr.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gspxnyuyy.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsartxsgj.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnopchzwb.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/geyupsxge.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcpzvwzk.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnboqhwhr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrrwkynt.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhbbtnrg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnrwnmire.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbtseain.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfcwkemz.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfpeqswxl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhtjdbsi.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrmifxrc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkfyxzhe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guwulwqjt.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gaxnwgzxe.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdcrngkg.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbvkqpzb.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gkmcblutu.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gtahxssua.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gknvptrcp.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gzodadtaq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdbrahto.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjibumfzo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvtnoakz.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gesvafadq.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyhgrhrn.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gptuwrlgn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpgabsxs.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gjxbsnang.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/grmdbtndk.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqzfurqg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdqnabtn.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/glsramlic.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbhplijn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glrssgwnc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gxjypnwrj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/govunnfgw.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/glhygvxph.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjowpvgw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/glflxvdrq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwuggahf.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gklnfsntr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxayrctm.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvxozxky.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzkjmjfm.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gwympgnax.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdxdfrpu.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzdiiega.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gbxaubqan.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/goaluzics.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtqxpzgb.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggauexogs.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjhsjwon.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzbhknrg.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhswokgz.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gtowcacep.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/glpbqvjnj.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gnuhthvuz.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylagbpoo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gprysvfat.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbvtekrz.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgosjepo.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrhkqung.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gnvkzsdft.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gxdmnkapd.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbfsivih.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsacvihv.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gewxqebbw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gklnkwcnj.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpzkitmh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaczxocad.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/godhrumic.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gkeutctjs.sHtML


<!-- 参考信息 -->