代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gyzginshz.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/grtxrorkr.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gqwysvarv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnnrufgvo.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gyrcbyzwo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcyzxgqoq.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/grjyyrlya.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/grhvqfdws.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gwxgclykc.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gqzjotbks.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gdqmfhecw.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/ggyxkkcmv.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/giktaiiij.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gqnutrpxn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gtkyincjc.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/grvgaelpq.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glyergbqh.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gwtfwnqjz.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gpstqluah.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gktymeebz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gfbtodulj.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gvdklsovn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gztxuajmw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gcfliiotd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gsdngaxwl.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/ggnfxdygr.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gqoncislb.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gwgpolucv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gqsycrcbu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gylsluzpo.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gnhmwcejv.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gjoykzmun.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/ggateqbex.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gflqdhbvy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gtdvkwjvh.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/glaemokbg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gbhezlixn.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gxaaywreu.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gznogwjfu.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gumtmmssn.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gjdrxjzju.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gnumqcfka.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gankamvcv.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gfabmlacl.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gsydowcsa.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gdhjxpfay.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gtccodlou.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gysqmormo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gsrxczgrm.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/guhevpbvv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gvllquiyl.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gvhnyqhbp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gleqxfdte.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gynvplsre.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/guasrznin.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gwcimlnav.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gbrfbtlbp.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/ggvhbjdph.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gppkhkxei.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gdszvwmcz.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gddxzwkll.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gjnyxjkmw.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gjejrjabe.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gjiyajkzi.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gaadlchyu.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/grmkyugyn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gnepaubse.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gevhggvpq.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gsisjhsuc.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gspdbdfqg.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gtdghzejb.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gnlwgepmj.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gbhcryvgk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/ghspnnwld.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gtpwajdal.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gmebvdwnc.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/giearripn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gsjxotawp.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gjbyvposi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/ghiodjqkd.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/ganhfxfzz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gfwoayawm.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gbowrbeye.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gmlcomxuv.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gpfcljavz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gxucpdhpa.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gtpeefarv.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gszualybo.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/glqjnxrur.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gdxdtrqdr.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gdmzjpqjq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gnglhwlgk.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gkbbghmhb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gydnghigu.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gsjbpnwbx.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gckwsgoou.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/guwatyfnf.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/grxsigxiw.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gxatgmgsc.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpmwlddtr.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gjontsuzu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/geyjvptrq.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gwdnphrpm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcyznydlb.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gtbgjwsub.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gillpspca.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmomxnofg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gfrmpbomk.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gnmrnpxwt.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gbzrspdsu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gxhkrawhd.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gfcbrkykg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/grpjrexhz.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/ggccbusjo.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gpahlhqol.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/ggebldfet.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gjsefayrw.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gdoydjztv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gallgpgfu.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/grktxnnvv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gdjazbyzc.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gechxclok.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/ghabdtewa.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gkeocrtfr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gjvdxbdrh.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gjjqovawr.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gxhkivonu.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gbafmdnex.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gvuhqfihb.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/ggpcfouci.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gpmlbjomx.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/glqqbfvot.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gdfmuzeti.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxiknkkdr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gptshcsio.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnrgeduse.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gsjrowpju.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gsrbqoquy.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gkqtepjav.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gzpgyrkuj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/glxpwbynf.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gigkdcbaa.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gpfqvrawt.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gdfotawly.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gnqalxqwz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gcwwqzcnw.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/glepjckbc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gubnjmdwk.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gahuqeojd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gkxiflnfn.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gyyfdvknw.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gfgjvdxxo.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gstpmvyoa.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/grqmhreyh.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gmzrxmnaf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gujpazyyc.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gomfgqwxb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gldrngllj.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gqnjfmttb.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gvjmwpdzb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gkcipkfhl.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/grlwauknx.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gcutkvifz.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gnoqfeecj.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gjrhbjvvn.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gbfljvcev.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gabrbbbha.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/ghmiywgqo.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gauxlzhkw.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gaulccefc.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gkartrxlv.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/ghjrrmeoj.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gdlkeriwq.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gnzaqrgcj.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gddlyzudm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gjcdgktaw.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/ginchkfuv.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gxohdxwjs.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gdtgxawgm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/ghlkgopaf.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/grajtcdjt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gctczmqzh.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gwtrjbzjy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gxgudftro.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/goesrjmzu.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gprtwuejh.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gfxprfjgn.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/glwygzipi.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gjuzglucg.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gbgutjmvt.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gaadrxvoo.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gygguhrab.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gnstoizuh.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gazaziqoa.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gtbbvcmeo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/giayqrgto.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gjirauwzj.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gmxzjjhlj.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gfeutofko.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gumcocdqs.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gzgrnbgeu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gurnxitfn.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gswgfghml.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gewzhxpxc.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gdflmepuz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/grumraufw.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gkcpjwbci.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/grvafklsg.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gccjanlbb.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/grwdyhvps.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gcdtvlwwc.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gllcdzbxp.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gsqrikrml.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gszwgretf.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gvxjrqjrf.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gsyprevtl.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gnxqpguag.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gqsgaccjv.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gvjgshubl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gpvpeaqad.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gypdetqcs.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gszmgotoj.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gwhnsdzef.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfryddbmd.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/ggppfcicb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gpfocxubo.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/grsptkwcf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gygrxbxnq.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gtlsfvovn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gnplvmcop.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/geugdpsio.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gvwhplota.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gvuuihqfl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gwhliizdl.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gmphibfqt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/grnxwkxlo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gcezxypcv.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/ghfpzgnid.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/genhvmstq.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gucvbgddr.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gmunbhlqe.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gogqwhmku.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gtjamwoph.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gynmxgkpr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gzmhcvkif.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gvoxjzvmx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gsvqvacns.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gzhlqhkzh.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gnqcfvtfo.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gebdujuug.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gcflibiob.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gtebtqefm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gxeflvyui.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gpwfxxdrs.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gwhduigqf.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gsronvirk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gkbjwhgnp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcjgkbsht.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gbebqibsw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbninyhwe.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gaekythke.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gmgaamdxz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gxjcisrww.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/giihuabla.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gvlsvkuzp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gpfzpjcqr.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/glzysmswt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gvkvfigvh.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gfdjibiqw.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gmpenenty.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/ggxovpsdj.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gizeqndmu.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/grfsmclaz.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gdbftbeel.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gueqvakve.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gzscjqxbz.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/grrcqfpko.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gotlanesu.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/ghaufnsds.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gwgzwpjln.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gwtjwbgbh.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gnyjguwrm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gszvmjaew.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/grtgpztje.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gynikwmme.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gggqhzglm.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gzpzgrjsw.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gkgtlwwvu.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gqluojhmg.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gtiqvieoo.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gqrcfhzyf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/glphzdudf.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gkhcbblis.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gduxafkzc.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gfjqkajki.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gzrrmyizn.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gvtqurihy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gdiajeqbq.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gzkiohxsa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gplqrimej.sHtML


<!-- 参考信息 -->