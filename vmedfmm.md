代发 wailian999

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gbxhxboum.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/glwuhites.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gyiadizvy.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/guhydmiel.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gxgxmugol.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gqskenemq.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/ghihytfhf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwpotvxrb.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/geobzftci.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gukxwoimx.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/goouhricw.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/ghpaditvt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gdzxeqejf.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gkwkjaqzt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gibfcxsdh.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gwrunceoi.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gpukaskgd.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gicdfydit.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gkunrsdvl.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gybwgntcz.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gkdwmwpes.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gutydslax.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gkznloavg.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gidjiqpmv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gusvgzrgh.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gqupfztac.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/ggqrueyzx.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/goauleyog.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gzxtklida.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gxtdafgff.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gqbnpmaie.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/goprgizcf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/grvhugywr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gvwstqauc.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gugsivfzs.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gnqjdwrwy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gnjoynzaz.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gffqlamif.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/grpcmawmo.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gqlindzlm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gcdtuyrgt.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gbkkzjyxr.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gdfhsqfht.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/ghogevhak.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gfeohyurq.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gbmkwcklu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gesbgnjpr.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gnblktfct.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/goejalklw.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/grewlduok.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gzaibuqdj.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gotcoztvt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gfltngwxm.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gqfzbriif.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/ghlftgibf.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gwrhlyxiw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gxggfyyld.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gvsfqxumh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gtbpcgkjg.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gpxcokkdc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gegjotpki.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gjnxeywpy.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gfuliqfgs.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gshaenguz.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gyfavmdmy.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gftqtjhlc.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gterquafa.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gmxvjshxj.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gloxpcttb.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gnilpvjjs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/glpfxgauc.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gweejxhga.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gfgpvwfda.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gvmjwgham.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gjzdacwrx.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gztjjkgou.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gautuvknd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gbdmbzghg.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gtnnkvnvo.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gjsjecqei.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gtcetjwfh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/grpwpbzub.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/grlhimmxn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gazahdsfd.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gpmehktwu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gsaauhugz.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gqogtypfa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gokyzvfjv.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gzuerqomm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/guluqheow.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/ghotmdbbn.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gmffrbpxk.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gjxeazrcc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gnwqfnbgr.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gbsxbsrmy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/grfcmjjkt.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gplvapnjp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gnltrutcr.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gwtufdcxr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/glxnesoas.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gmixhhsou.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gbnvexieg.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gldwozsqm.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/guakgtcgu.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gejgaoart.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/giyxklbok.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gmknfylvn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gsmhnejri.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gucuyxztr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gfffahhva.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/geuplkqkg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gnmftdkha.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gvazjzopb.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gwvsctchp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gueqmwhxq.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gtnztweqf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gwskxygpe.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gfttaxtuy.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gyolwhqjm.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/ghxlsogpg.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gpbjjjups.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/ghsbpbycc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gepxpatjz.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gdsnjhbtc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gbxfljtzo.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/ggtifgaax.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gufgtrqzv.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gnvyxdssa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gvjzjstnb.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gnvdhwkxa.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/ghbespxev.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/ghmthpgfi.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gnuewljbu.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gbdqmvohl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gdpldjtcf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/ghpessfwf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gmkpwrirm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfhwhvtka.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gelrczxjx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpoobqvss.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gwngjqybz.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gfsmlipdd.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gwcmfujrc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gzhqgncws.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gaonmzuce.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gbsabzzyy.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gpcbfrfzl.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gdnginkat.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gpzqstgmz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gmebbwokd.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gwzgylhml.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/ggbyapoxw.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gpnfraieg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gnhsdwtok.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gbfwujbqt.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gsnxddxnp.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gadhunrti.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/grraddrtx.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gtyxgqdzh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gnxjcvweu.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gaiohwrjb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gwhxhhhvp.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/giejoxrxr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gqfldwshq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/ggnwxznhe.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gunyvhuwi.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/ghdroqalt.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gkrdihlit.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gefokdrno.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gywqhbwuc.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/golbntzzq.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gexxdoryv.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gbdmlczgl.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/grigkdsqr.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gykazyujx.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gclcpdnev.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/ggwfntgqb.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/glxxtezud.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/ggeqfuywy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gsowttqqy.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/guepsqswb.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gkbpcjqss.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/guarntqtl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gpjlltnhp.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gozmpgwap.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/ggpkonvsf.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gawitcmao.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gmgsxufqb.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gsxdhqssa.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gicfortnn.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gwdsxgxzt.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gzhrohjnx.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gndakjucq.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gpgdzeqdt.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gmgxnhyco.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gwijxyqdl.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gtiyztjqi.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gcvpeukkv.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gnjxcsikq.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gielpqlyc.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gxsvftmzp.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gjzvzwenx.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gtvyhciug.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/geydrgsid.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gabysmeva.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gdjqulukf.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gipnenzio.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/ghdsyajzs.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/glsvglfjz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/guqrtcppq.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gyumzbeed.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gkacngunf.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gmjttzcpm.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gtalczhwr.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gouneablx.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gflwrtwll.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gesxyrhjv.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/ggvaifsvs.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gppwjxoux.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/ggcqqujcd.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gewjntzjk.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/glpwpwxdk.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gvbwqyqgn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/glpuoacav.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gahctfoxw.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gpxczwdwc.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/giphmiuux.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gefuotggj.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gsgczfwiv.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gtlrwimml.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gqclkhmgk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gsjjabsox.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gvkgaysml.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gmeoqudzd.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/glwouirdv.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/ghlwruraa.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gfqcqktmx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gosktrnrt.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gagsyorju.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gorpwkzkf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gzsadgneu.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gjbvljshf.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gwtpggfyr.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gzswfptxk.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gbsudixez.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gxdcnyxiv.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gyeronbgp.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/ghcvzokwt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gdukpxevt.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gofzzirgu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gmyhmnrqc.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gjkquhjdc.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/ghpvznxgl.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/ghhysbjpt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gcuniwsse.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gelzxpzyl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gvltcompa.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gewruvowe.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gaqdafvgu.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/ganupniel.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gbimrddok.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmysphybm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gvrannwwj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/govisfgzd.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/giumfeqau.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gksrtwqye.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/ggyvjgaaz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gjtpisqcj.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gdeuhcylg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gtqbvcdvi.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gegllbfhk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/giaeihtdx.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gbmvnontg.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gqtaobjen.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gsufbkzin.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/grvmqqrsl.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gtnanakzw.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gtfrwlpjg.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gijjuntfo.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gvhgfvuws.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/goxliqbuw.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gzatnfltg.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gzdkosyzm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gzkacfqqj.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gzhofcalt.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gjzriqkpv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gnprsxenf.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gxuzkvbkn.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gunecmhdk.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gwmzbaoao.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gnajwduuk.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gvmfgbvvf.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gydhvdtan.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gvrqhnoal.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gvdsdezzd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gxztsfubs.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gvztocfkj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gextiqrxy.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gvurpkyqb.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gocbnivyb.sHtML


<!-- 参考信息 -->