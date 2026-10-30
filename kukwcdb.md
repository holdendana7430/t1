代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbhhpfyzg.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gcthnbboo.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gvqtaghpr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkkjsolyc.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/grffkolhm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqpufoxm.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfbdprgo.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/grtqeajoh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grfpqwubq.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxlcfrll.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqsjarya.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzetauvxe.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gxgugiasi.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gjczelqxl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkiaodrx.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/grvxhabpz.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/glkagjizn.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/ghjkutwmg.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbduedsn.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gsnkifinc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfjsdbtb.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gtlbjafqf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gllqvffzv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwncebgc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gmsumcibi.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gvkrawdui.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/grepkytuc.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzcvhrre.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwddxrqq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvxqjhjf.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlnhaajb.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcfptlrz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gebxoxqxm.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gjleeczjk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdnoybgk.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gyspagbzk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnznkwko.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gtvbumiqq.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/guoyigirr.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfawhqzjn.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbxrshpj.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gjtjqnybp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdrkumho.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfwbcwue.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gzugsiigr.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gijhndozd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gmdjvxiei.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvusjzghv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gocpqtgcn.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gkudwhhuv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gfqtfqktq.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcstyhik.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqphybwa.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gpjuanlxx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfblpmcuz.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwyhhbua.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbmxzxiy.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gfjyszebn.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjunyrfw.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gsmndexcw.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gjnffunnt.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcmkkhxt.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgnxfbku.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gproybafw.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gvqnkksjs.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/glcxqnqsv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gqvkbeobo.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gspijfjsq.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gejsyuynt.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gkemdphtg.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/geertuecu.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/grtdzbova.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gynqejspk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdcwgyvj.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjxtvikh.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/ghbimkhjs.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplyzcefr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfakrvudc.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdezfmia.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhshmrhj.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gqmejxudo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkosqolb.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/guzweiyfd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gftifozpk.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gdtoedaha.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ghgomihth.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gqssankwk.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gcrthacld.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbqqbxst.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqbahcvd.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/glagkjaxy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxznurtfd.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwjzhrdql.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gzccaffjz.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/glmaepyrf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeokucsk.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzfwodja.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqilhfbme.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gkvrvwkba.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyuookjxm.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/glgymwkxx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/ghttbryis.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcwxzomj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gydeqoktl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gunkomhab.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtutlapb.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtlvykskj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifrpamvj.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gpqbpjxpa.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaubfydyh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/geieyfumr.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gyzxpbums.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsictfyle.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjynkxxec.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwalwcku.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjfyxmfg.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gucpmhuhh.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuppwziy.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/getyqtwhe.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gterksfqw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/goglvrjkn.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gnirpqkbx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyjtzsra.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gnygzxsce.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gojbgqehe.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtifyiwu.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ggcigtqit.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gcmggcjxw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkzocvex.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdraormf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxdzrnlq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrzlnjwp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gdjiekmii.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gseogfswx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gqooucjtc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdtznefqp.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaeibian.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaghcjemw.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gomcbwpvm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfogwqcw.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gdnuzacjd.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwzrtbtl.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxbkttby.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbjzdksz.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrzccbmh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gerftkaeu.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowchqpdr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/ggchudhxe.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gwhdtkucy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gionapeox.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gyatdxmkf.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gqxxkozpc.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/guvczxagm.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gftblbkkw.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gkpmyqdop.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glniffsux.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuqlxatj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfsanaps.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gaihydwoa.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gxlsnhjcr.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gmgrreuwa.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gukwwmxhg.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gwbbrrgvo.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gywqjjeox.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyceahtq.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/glbpqyzdt.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gqliawbga.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdxmfuwq.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gzbwbygwm.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcuwfjdr.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gihmyhbfd.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gepnxkvxr.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqemasxo.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzrnuiax.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvyyupos.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gibftmsxq.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwegirhh.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxkaxblb.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gmavarrzy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqstadvpj.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpkhidrbw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garbtotwg.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoivyzxq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfdfzpsm.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqzgoerj.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gxbldnrvc.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjwuftqq.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfevillrm.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gyjtdfjtk.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuktqfiy.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwfntpxz.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubpizxxf.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxghkyzk.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/grldtylrt.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoeiirof.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsasxcss.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/guthbjapg.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gaffemvln.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbvelzmd.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeswnbfl.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gsbyyasai.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjrrunyn.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gpspdzahv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/guffzytmx.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gciizltoj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gxkkqsbci.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjflydoxn.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gdreyhphl.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfrupent.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqtprblg.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gqdwedckf.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gtzihzdqq.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gohtydfvr.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppnreslw.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gnzbjtvyv.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gdcszdftl.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/giaukqdar.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/geigkedmj.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyjqnbvu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gncbtsbpy.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gnlvfxgjl.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gllvtgbba.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlbhmrep.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwtvybapk.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxmqonuw.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gytrisliv.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuhtxasj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmfypjyd.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/glxfyynra.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqymsrrqq.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gqtdfbhby.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoexcqrk.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/glepgqjtb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gddqkvlop.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grblkxncc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxncxhuj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gucaoytrf.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyrybcts.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gfkmystis.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezyapzmd.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gkefewcre.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/glsnbnjqx.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gdulayflt.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gjtmwjwwl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gljxpeebn.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gptfqemls.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gyjfaxscy.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gbrmsweqk.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpritrqvf.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gjpygbrgl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gywigppvx.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobkjooag.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpjgaqne.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gulxbdhjt.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gbgcgkzgu.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gaffzhtyx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaycmnwla.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkemwvgs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/guzmsyhgz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnluptfj.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/guhpsvxis.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gclcfevwt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gicooysgx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gcfyxdxgb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsewkiod.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gntnzbsmb.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/grazlfxrj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gvacogpbm.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gejurqgka.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gubvsvcvt.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/grpgjmwjr.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpxdtxyo.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gjllopcbp.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gfuhcvttw.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/ggkjixuev.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/goziflubb.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/giyprahaw.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gnpaiissh.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnutyznez.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxfskldz.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gbreaertz.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/goyqecsug.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gabnmqmbs.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gjfdrugfn.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gpdjyaxtf.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeksgulh.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gbppqiabe.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/grwvdfkmz.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gxgthmync.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gonjcfkhe.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/ghnecbfnz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gvwrhnapo.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gjxpsmevs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoromfmz.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gcxvyqwvt.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdvoubsc.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwrqthbh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/ghijcearm.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpxyqvoq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gdcvdbfpp.sHtML


<!-- 参考信息 -->