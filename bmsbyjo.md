代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsjotdsx.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnynlveko.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyevaknj.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdyzisnk.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvzayqtj.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkvzsspy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqdftpox.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzzxoyxg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gwoijoaeo.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gddmdigti.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gzpigkywr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/goskltjsn.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gqeseifjn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbalheqfs.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gtumrfpua.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grblvforr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlahwlel.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gdxaounaa.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gfqxafoeg.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gsvmhtteq.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gnpsllnhy.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkitedzpe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/giwwcfrex.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gdrcyersi.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/groplvuss.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcdgwmky.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoboipqy.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gfcpehvnq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gkipjlgei.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzwgvkql.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gegentvtx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqzxejyw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gjydipxxe.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gllghysfi.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjdalkox.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gaacyewvm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gfulstzzf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyzrveib.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuvmugvl.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gaunohfpd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gmypnredt.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gmvnqelfq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/glvsignhi.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhnnmsan.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gsukxgikj.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvpwuedx.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gfvvgtvgw.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gxnyexkmn.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gvxqygwyh.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqwzsscn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gaogcohen.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gsoffgcoy.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdthmlxji.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gzwjiguql.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gerkqchww.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gtndzjjxf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gypljiows.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gbqczhwwn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoqlygcf.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gzpfjqxkp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gnmuuevvu.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/grjczlgrv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gakodkmys.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gurbkkjxb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gavliamvg.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gbkighekr.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvrfzsiu.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/glqzwietp.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gntagsdjb.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gdqzwgrze.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueoizmiu.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuwrtvul.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gtzvkfdfs.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvcfzihru.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gflmkvqtp.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkcqrwjh.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gqmqnscmy.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/guhjmcvwp.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gxonxqhec.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gzavvmxgg.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/ghjnflays.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjuvrigj.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbdqgdov.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzqrmicm.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gkdelncvp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gnrvrmyky.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gswlrzupa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyitawmlu.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gphsjzkkb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjlrxtxi.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gcnkxtpyn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gdplpmkcg.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicrwoohv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gwuorncov.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gkfhugiut.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/goymexurb.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnltlewn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gvofbanep.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/goycqajvc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gfpsnlduo.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqaeodkkk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvruniqfk.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkwwfuuz.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gymcorpch.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtesqkvs.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gugfnhmuh.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gimhgurke.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gykssfvik.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gaddlehrl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmasautj.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvqqprqs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnavscef.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gpapdmgvz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwwzgdsf.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggrnutaxh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gldpxtcpu.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhulqclo.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gatpqcikd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/geprbousn.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmzkirkf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjytnuhx.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxkiubpi.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipobtdlw.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsudbfua.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbhsqaik.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqojllse.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkkwrpkj.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/ggusithvu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/garwjstoy.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gpoxvjapp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyaejqqz.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoqyqkdq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvrmlhtl.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/grpyuhqgj.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gthcrvtfm.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gineevbet.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtlnaiov.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gyxiwbhnk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gzllzqvug.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gfbysvadj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqcjfuvh.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbncebvh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrvqyxtj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkczfjuqx.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfcndxwh.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gddhtijdv.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/glecbgruj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gjwamyqge.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/ggawmopwt.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gczeyuqax.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gjrkyunws.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/giwmldqrf.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gwanzrpxt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gvgozbuxm.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyhtmulw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghviansrw.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/ggdtpomgc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gvngabvjj.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclbscybz.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/glixvvfzd.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaljczmn.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/ggldkozdj.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzslvirg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxggcjft.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gnacvziqp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqfcucxw.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/ghlqoiguj.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gyrdzccrf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyrjwukr.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsugqikci.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/guvjdgrqu.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxluupkes.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbwohxsw.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkmzogtr.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gffqenegz.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgcydrjl.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggommlauy.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ghahxigft.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gtwaicobc.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gcpastlok.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/guqqzasmn.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gvrfejvsn.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqwrysse.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkchuxqj.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeotaaxx.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvktrrvg.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwrcsqhp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgzqqgkh.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gpxbmggul.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyrdpxeb.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gtttvnfkm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gcgrhfdsm.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gvmpohmtf.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdnnifjj.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgxcfoon.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuslvmkd.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbnxzhgp.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gtrfjjzav.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwknevjic.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyabpydyo.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgfieogz.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gmlefjpeq.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gwkzsvhss.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gafsielqd.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gymwculad.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gckecxkny.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gorwbofzu.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/ghxkevhqe.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gorleuclg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhrafhba.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gqoawrrax.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/geeuyvnku.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gowjhzbvk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gonbtrgar.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gquudrkjn.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtyimiwb.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gbajiahpm.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsljmubgi.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gzxlevujv.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuqllkxg.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gmqavnnts.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/griaracmc.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gkmpglgln.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gllhsourj.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gknczcxkh.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gkuzqwyif.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvodoeee.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoyuifyp.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/godjmawoi.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/garewekko.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gzinvfsre.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzujeskxa.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gnjakfbed.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gawymttft.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/guojohgsa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghlvsuffs.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gmazqdgck.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnohasbwr.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gaqqhcaqh.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsjvdqjq.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpxatszrt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsgtsmkt.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdismuaen.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/geqftdrdv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggehmktht.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdnwgtez.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/guvzekkoy.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gimbnhfgb.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/grbvepxqu.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoopuata.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gjniirbce.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrokhjir.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gkgjbysjp.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/ghobgknzl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrshiyrr.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrbodbcb.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyiwmptk.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gffbsnhmb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gdzgexbjx.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gxavikxdh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gvutrhjwv.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyujlbgq.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/ggqbtczgp.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gvizltwmj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqozdabma.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkhzbdnmp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnitfbloy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjsbiycr.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gsojtilkn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gclrrvzaq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gtakdvtpc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzsfcvuz.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/grkliemkv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/guyzzmluz.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gmwjsaovu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhcynrgg.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giocbyzvv.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geszybwpt.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gstoptwyx.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsuqmmur.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gokbshjlc.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gthmfntbj.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnvntecw.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmzkmivg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gpebdytlc.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghojuqpvl.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtydcqfe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbtoqiih.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcdzkgpv.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxhfwtlw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonjiujqs.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gfmkfsvws.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gcughbwis.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gybcfqcyd.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gombporkd.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfqgymha.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gxsycdzex.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnniyodbf.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnoskhym.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gpksasbwt.sHtML


<!-- 参考信息 -->