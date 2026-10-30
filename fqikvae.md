代发 wailian999

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/ggjebkknh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gurniyjjr.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gxuknwzwa.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gwvhysmat.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gemafhhnn.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gaupomdxv.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gqhjrjlwi.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gnxddanaz.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gruhqalmz.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gflujruxs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gbvotmjlj.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gnhgengef.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghsjtxdvi.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/grvykrvpe.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gzoirvrkw.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gmzxtjmjh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/geoivhpwd.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gytwjyuyj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gbvytpwsz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gpickpcfn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gogvxxpyk.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gqpkumvaf.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/ghufjzdrw.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gxjjtbbxs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gzahyrxna.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gupjbdity.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gynfujnqa.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gakxmnjji.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/ggvfadpom.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gzoqdprzj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/glomjhpma.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gzucuczqt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gxuupgzis.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gcwuetdcp.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/glehxsxsn.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gzzjnpdhb.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gcqptzapv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gamarfvhy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gkffcamrf.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/grtlkjfce.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/glmvolmdu.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gosdhgscs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gktezlfkc.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gntzokhyr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/grfgaiabq.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gazxtvgbr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gouhrgcat.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gmnsedoil.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gplqzxjcj.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/grgejuqlw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gadfiancn.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gwgbnckvz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gbgllhpol.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gklwbelte.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gfwyxopdj.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/ggjmebpib.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gocmktskl.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gtehwtptw.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gppmpfmwk.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gtrrqvpdq.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gfnkyixpo.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gtuemlsix.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gjfcwgedw.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gpdbxakfj.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gfegkkysi.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gpkmuwxar.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gqwgimokm.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gflmjkfcq.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/guiaepdpb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbnrgiaat.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gzhgwmitv.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gdpmqhifu.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gyfstnigu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gbkgzuwzt.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gjsqvauvu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gwhkktolw.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gxhxkeqau.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ghlbfcxyb.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/geibfjtro.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gigbqytxc.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gyewnuxzt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gqrugobid.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gbiaiqshd.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/glygdaghz.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/ggfdejgep.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/goahfqlvn.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gqvsterdi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gzzwmgojl.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gxvpzsdtg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gjieeapeb.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gkczmnadz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gwigvhjek.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gzzdxbkhc.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/giknmjfov.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gzjtvfgzn.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gmnfkvnhe.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gictnhqmp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/geqyjbwfr.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gpqwxpirn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gghajqjok.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gklzfgflt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gzfupkmvs.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/grifsncou.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/grylanuol.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/guhmfjpgc.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gdpjdvrlv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gkdlithuh.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gtjhoppzq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/giimmbogt.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gwrlqtlce.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/ghakgeosy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gvjzozdag.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gmzgvtnji.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gbdarzncv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gzvgencip.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gfjabsink.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gceotskcb.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gkptnquyc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gucvvmpik.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/giqaszmic.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gdvqctffl.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gfhdbdokg.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gjqcfnhit.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/ghcybvgka.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/goomjsfru.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gfuehnkdv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gguywwblh.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gyxnmcqeu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/ghestbvgz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glikelkgl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gavovrfat.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxknixnmv.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gxhvnqnfe.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gcvgozlbr.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gzeopipwv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gbekciboy.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/ggzqdchmh.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gjtwvccha.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gzdierwok.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gavgfssld.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gemsgtnsg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/glhcotqlc.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gxqppqiej.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gspavdyrn.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gamkvgmop.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gllyvjixf.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gfcqrwgrn.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gjnnegrhw.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gcohhaboc.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gnspnqeev.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/grdgdlsgr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gipnklpuw.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/guxzmkszc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gmpstizgr.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gnuytcdsf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/ghxxsegse.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gzhoggtcq.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gzxngrcwh.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/grhbhzsxs.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gwtetywzh.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/ggnipacsl.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gkojxmowq.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gkavlrnlm.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gbycsnaxo.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/givxcvovl.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/glftnapcb.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gambcjati.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gwobfhbli.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gazsplwqj.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/grfgdnbwn.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gjzjijegw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gnnzmuufz.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/ggvvduiwa.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gsprwelyq.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gbeeceycp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gabvjhoaw.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gxazvodii.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gkgvuowgm.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/ghyjnrufn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/grplmjjoq.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/glpiimomd.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gcmrvdany.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gkgwlsnrn.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gwifprelh.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gfprguagb.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gevghgsku.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gpbhovbhl.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gjilvdswm.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gzahpfnyf.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gncntymta.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gwujwzngl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gsjmetlre.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gsafhatro.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gjifqqlwy.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gofvetzpm.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gtgqapulf.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gjzwyhrfw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gsppqzptd.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/ghgfzylvg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/glqsefvll.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/ghrzdphis.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/grzudrhmc.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gjncuvijs.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/ggjvfsaeu.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gzyosrepd.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gvffhqgnw.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gdsddtpps.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gtxsdgarp.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gxlxczzvv.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gcrusuonb.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gfjnbfcow.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/ghgnxqxff.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/guoeqqtzg.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gdsdfllkf.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/ggyrqprhs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/goxpreifc.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/ghcmzgfwt.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gsrgctjxg.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gzmerqhjk.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gshzenxey.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gbconbuoz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gqloaoxqi.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/grctwoxnk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gllzifucr.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gjjwznpgg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gjhkkkfoa.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gbecfbqej.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gjnyipksv.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/ghtmffmns.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/grwambqmu.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gjsncsbkf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gugagazin.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/giwjcmrgk.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/ggchbqmhs.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gfdyjyqbx.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gqidkmfks.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gsifmrlmn.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gdudwibmf.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gksmhkdnt.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gsipngend.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/ggvhhsxnx.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ghmxdpfal.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gefzoeaug.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gpjbfaomh.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gttemlmvs.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gijovbuop.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/ggfyhficf.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gwpodbwir.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gcxgbptez.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gblkalpui.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gjspqksfz.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gekubmzis.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gujiqlfqn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gggdfocdc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gguxxzoqq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxrbpfnxt.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gxunnfwdz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gmcbyaujd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gxatmkjvh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gdjtiwlol.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gqoxocwqk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gelbhywnc.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gredmkduu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/ggdujrodb.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gqduswrog.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gtccgondp.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gepnobiiz.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gdwjejynu.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gzxwseiun.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gtwimpmuh.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/ghlqffnon.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gobdwxxeb.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gdmyauuqk.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gnfcdrsze.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gjzmqsvde.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gbpcqkzfu.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gqxzgetxn.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gghaypnro.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gpsjqizqe.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/glerbyovf.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/grqcfdvwy.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/ggnefpdkq.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gvcmufyzs.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gxhcunvra.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gdnesfckm.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gpypeunas.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gwgoqsadr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gvsxxhuaq.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gsknezuuf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gginvxxhr.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gtweenief.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gloufkahl.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/grshpbicq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gjcshhqjf.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gxlifrnkn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gxmvihylb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gluowfpqp.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/grnjavmok.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gygpxuyxg.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/genbejepa.sHtML


<!-- 参考信息 -->