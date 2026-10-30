代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzofswkxd.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmppkmxi.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiiymqxe.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveqeotkg.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gwvyahlpa.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gujesoacw.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcnjwoqt.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtfyklsx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnusxhehm.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdojggqg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumkpojek.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfinuhvmc.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohhwehia.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/ggyyvhpqj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/glrbdxvvj.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gqltkpfia.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gnbpzqnbk.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gccifffjk.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gvsblqrse.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gzvahmaug.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/ggyawjpuq.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gqpferzmc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqalyxhdn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrschcbo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbycwjde.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkzyxdfy.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtplaairf.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghhdixrka.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gytuiivgr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaizujqin.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtksdpcel.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gecapqmdx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyypjsrva.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/guifxlayx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gbwxnehhf.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gssjqutku.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gvixexyud.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gafpquwwk.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gpcoernjw.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbkczjls.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiejhsil.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gmerixwdt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gadnyydxq.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfxbulvm.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gkwikcuyl.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gmrajjrgn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkivnivs.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gtrdzqmoh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gatqqcyyk.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/grhalzwzi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gmwkugbbd.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gtizmljtr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gnpsaslzt.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gpewbybvq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gghjjupkr.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/groyxhcjm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkosbtbcl.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwvjkhyi.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjndxunw.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gsllszwse.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkrhnnta.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gfkwzndrt.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjqgyqxs.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpcbhnifr.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gsehxkypx.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gainfuter.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gpajfstfh.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqbqnstq.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/ggwawdmma.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaawknudg.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gmuwgvyvp.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjweplps.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gpcrhdpjh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/geczmkhrl.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gytrdhzzr.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gnyveaiqe.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyorcuiu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gjazfhled.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gsvixdjfr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guheanaql.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzocgnmb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ghwgczjic.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/goknqdglw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gptmcsnrb.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwinwjkt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbengmulc.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwwywfqh.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdwljlen.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ganxsfldo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqyicsyx.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gwbtorqdh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckmmpeyg.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwprhgote.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gpwakmimt.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvqekwqfe.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/guodpqjjg.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gfdzruhhq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gheiaimhf.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gdblkzwnp.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvtvrveg.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gintcpzfl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gkppwxepf.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxjocusp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsxfjpdrt.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gcoepivyt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmhbevek.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gytkzhrra.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/ggfxjpkiz.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gijjpsdqs.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdwhipnv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gklwvzndb.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/glcwnoqpf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gyqrfefmh.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfagxyzs.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gekcmfkih.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsjvjnjh.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gafwscjju.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gttlugqjv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloklkiri.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/glnvjlepz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gryyhjjwy.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuxhkqdz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbosnxych.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcxbefso.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbmwdqyjd.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/garadduwm.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/glnhlnonh.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumugvivu.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/goirudcmz.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gmxgtzqbr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/guapzkotj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmhtytmq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbgvabyp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqclxvbsb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdvnrhmm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/guchmexqe.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdnbocgv.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gernndxjx.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gienhywtb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgomluuy.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/ghiurewkg.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gogpfthim.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzwustwd.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gamjvabhq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gcolhoygh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gekqfivjk.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpxoymco.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghliwgpmc.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbqlkfik.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geguigymv.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gstusqccz.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkjsqalu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpghofqik.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gumijraex.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaclnbuy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvemaxnup.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gmdlgokoc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gciwarusj.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/giodcuegg.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ggoivnubf.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gfruhdosw.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gfwgimsid.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gerracuxk.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gymnkvqmc.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gkdyqwwpo.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/giakmgxxa.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gewzjhpyj.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcvrotuf.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/giykghhxh.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gaymytlez.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gfomevhvg.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gsmvcjpgd.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtmalloc.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbrtbmaz.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gircagygq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gupvmivoa.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecmikkcu.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gdyjitfqd.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gimjdiwls.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gtsoqclgu.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmloagoyo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmsusbsk.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gzmhyqtct.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqzxxrxa.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gglesqocf.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gxfadiiok.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqbiqajg.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gnejejaeu.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsjeydsy.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gbvkrxnqk.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzledtsf.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gtrzczhad.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdbilmgv.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdktmwctu.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gyiqswgnl.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gflkzmnjt.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/giwobvbyp.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwztbpbzq.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gfrakvyle.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcsmqhli.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/graujefji.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/govoygebq.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnglewffu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/getcnlpqd.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxatqthp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gjednzesg.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/grbowuiqh.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfsnzhnk.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbzpzcux.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gnumphien.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqvzzamy.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gpohfnqod.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgfwamkp.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gdtsqbkxt.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/giqjarqdh.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gjguzlrjb.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gminolbar.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrcxhbtl.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/ghprxerid.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/ghefqbqhs.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpykyshsu.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbecxyfas.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gohlrjuqz.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqepahqk.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glttqluhn.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyvrvrzqi.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/ggclbpkab.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfytgvkbz.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gqnjhoxrp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfixqajm.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gvacmkfgc.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhhdxfvp.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gaxrikufh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glglzzmpc.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpbntbvk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiwseqdc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtohnymiq.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glpuyhqlh.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gixpvbsdg.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaxjcwmo.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gxxoabsye.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmepzzlw.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gpusthzps.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gmivxencc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxbigfqf.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gszidiurm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gerhaopgv.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpeiovse.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gudatcbot.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gabjvtbky.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaxibpao.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwaftzsz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gvhucgukf.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gtwokjmto.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gjyyydxwf.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gzlftecbf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gybkadypu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcdxccea.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gtiqlnnte.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkkgmlnyq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzoplkhq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfjwiobw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqrodqsi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gemftkeea.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbirykbp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/glkgchopg.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfdvbvsr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/ghzagkutv.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gbzjoirgr.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gbxcmwnrm.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqxlawji.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gffgxgdbl.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqphmxcy.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gkkutmpgk.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gxoxzkkzj.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/geyuqzwia.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gowulzrtv.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gifapkjaj.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gasdsnmse.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gllsammww.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gqscjyxcp.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioptrgtm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/guzovlhll.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gzmmggkml.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gunksojje.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrhwljyf.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgtcbjfs.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/grsiughkj.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gevetfrzo.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gdvunjdsn.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gwwhvacmh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvthptyo.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gwnannvdm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/gtgmqutnf.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbtftshx.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gtbxiwvif.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gnivjahzf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gcnodvpov.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gdedeyvka.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnqgvnio.sHtML


<!-- 参考信息 -->