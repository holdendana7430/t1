代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfzuwzvs.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmhnfibd.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gketlqvft.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfalxqqwg.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gmujlwwqu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgefimhp.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlwbudxc.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapsmpuxq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdzxwasr.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gllprudyi.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjocmxvb.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gkqbrnsii.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/ggekasgru.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/glqpxonhg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gwkoycfrb.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gdnavgesr.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gztxksvna.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gsiheynag.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcpbpuhz.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gwkoegldd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gtwbxdbqz.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gqsbpmmdb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdygogifv.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/giowrnlon.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxtgqhlo.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/geuzqwfnw.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gqtysmiyu.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geipizpoh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyunesok.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gwjkdzmcw.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gunnjyrfr.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmgkfkdy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gklthomyg.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgxrtpet.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gkaqwccdp.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/ggcfsgpxu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghegktdxb.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gwfbxiror.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gufmgpfbe.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gryljeynu.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpuktlqu.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gbqngyxwy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvlgztlj.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqorbhtz.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/guronblfj.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjewohok.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbigsqnfn.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gpvcamkly.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gcqbpdmwh.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gycnewabl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuuxgykz.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gamcsqdhg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gochprqgy.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyubjqrae.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gjambndsr.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzihfwlq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeecsmik.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gdsihwfwd.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhgfstns.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbgucsst.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/guxienlxz.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdacgkwji.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/grpewvczl.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/glgirxvvf.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gnrehtpnd.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaocbkug.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxakosind.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gyzdtgiho.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gylfflxsw.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/geothllqd.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gpgeicwsj.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gordaziip.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/glhlfpkbs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnjocmhwg.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyxpwyou.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/ghncjqikm.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidukgwer.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqwpdqwp.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gmsbarsdq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gngrunquf.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gbwwouphl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gosyugayv.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzubnctd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydccumps.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gfdkrmuju.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtgmpfzv.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/ghralgidw.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoancoby.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gxrmnawyz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyiyprqg.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gozxijjdr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnhehdsb.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdxmyhqy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipthceqz.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxmbobgvm.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gcdilchxd.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gdgqbtbis.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxmzisnp.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gmbjwazzm.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdvbhhxf.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gbpoymqmz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybryxuhp.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzfvdjil.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntzsleih.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbpwveim.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknmpsjzq.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzfbxeecn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gswdoxzea.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsttsiukv.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtfsqvps.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjffxamk.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gepacjtdz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gwvxbogub.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnhsgcya.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gniasybwv.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbsyeqax.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzorfikin.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gxdlfphkb.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqiojhvg.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gudbyppbp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/girtzsisl.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgqzixaq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdvyhrde.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gketnjulm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gycdooxib.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gbbksrbml.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/glwjdycbm.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gauvtgabm.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gfpcyvalc.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmanricv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gayxihqnz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixejjqve.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlwqpymy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnyisdzvw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gnondrpxw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gucihmsgs.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjmkwtjj.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gbccbpxce.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gycsblerh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsrdtazz.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gbqtcrrgc.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlllpnzf.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/ggpecshoh.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/geeyekzwv.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqgwkena.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/grfyedpjs.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gfetokaax.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gzllpbhks.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gjcivwmbl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvdxihkk.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggftvmani.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfijvwqbp.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnktewgup.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/glvzdalnr.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlymnlfy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzynqzidt.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/grfpnsoku.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtspbcpnx.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gjfsqznfw.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gqzsrbned.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gkekusepw.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gphqkbstq.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnsdqyih.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaueiphfi.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gcblrbram.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdjlugbj.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gjszlecia.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/ggpubojvy.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/girqgpuww.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gcgqyqnbd.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gdnvxycwz.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvbetvdu.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gdddyjzcs.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gelpplhlz.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/grwftuhma.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmefixvk.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ggrxbxumi.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genschwcf.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gphphqmce.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gyupnycka.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gunclgubr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gbfuseczy.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/glggjjmvi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gipwatdci.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/grkessgxd.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogvzseny.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaveukcgi.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/grizcmhkg.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwskpzbmw.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/ggxsppopc.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/grzzqerhz.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtrvaxsn.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gzbfvtozz.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gspfsvsnh.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyjlisuj.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gennmjrds.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gwwzksxdz.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gcbvzdprm.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggnuahyry.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gzptcwquj.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/guhagtauk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwffdxcl.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gmiardruh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbagqakjn.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxkyinwq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gdeydkwrf.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqowkveq.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkqbedqu.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxehgafk.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtrbxphi.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaqjvfzu.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gjeaidzko.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/graakundq.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gdwvicvba.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/grrwuhjvm.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gstalbcra.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/guimiynxb.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnjbmrsf.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gppndpnje.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gamteiupg.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gqyarjwxv.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/greuxzhvv.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqgkxojn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtrrijky.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdsesbze.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvoplqta.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gssqsugbp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjdvzssu.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gmrnrmcso.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gypvisbua.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmwihixfd.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhttbyje.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsisgrrgx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxwacvyfz.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkqiywfti.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiqchodk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmiazcsho.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ggfkjqhsx.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gohhbdaoz.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqglgywpl.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvzrnqaz.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbopulfb.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyocycqqc.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehsjrtjc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtypabfdy.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnyrlvto.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gewihoody.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gbcfxteeg.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxmlzppe.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjichugnr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gfkhwjoap.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwagybsg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/geyevepcl.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvyjouwt.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsvznmvn.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gtubkfffs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmlbmtnz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gutpfletp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gnlrjbdcs.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgedchhl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/ggowqrxnp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gqjrctizu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gshkbullq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsziwevpv.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gjzxwpybj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptihtpfa.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gollygsxu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrvtdfuc.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/geokusbmk.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzffxkulx.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmjovfab.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbafcngm.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gsepzylpb.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxtknzcx.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gcmmodqaw.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/gmrlvhjua.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyaczodc.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmldwoqn.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gnhyyhmma.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvztijcor.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxwgtnvs.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gwjrghjvv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpbearpw.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxccwbhd.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbdylrin.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/giyrbfgru.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/greewpxwm.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/glpvibtgl.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxaomfii.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcbzjrvn.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gavlyeewh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gyizhnjqz.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gmkumlbar.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqonjmpy.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/ggeqmzlgv.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gpysxlvht.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gknulxrhb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzhwnvyk.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/grirwwpkc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/giriqnjsj.sHtML


<!-- 参考信息 -->