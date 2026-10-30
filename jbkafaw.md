代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfejhcrl.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnecwbgj.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjoolemf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgibsuug.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgxhcmml.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhdlbgnv.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gvjukhcbc.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gjftbqdlk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqznphpwl.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhmxbzrn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gygbtjeka.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/grcfahhpa.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gommqlafg.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqveuykb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gutrwochl.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gowuiihlb.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwwdvrdb.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/ggbfynfsf.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gdihukacr.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuppemuh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gciozffxz.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdvhzwxv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnvstkph.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnfbdsqt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbsnumjv.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gjixhahdx.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpodyjkr.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqetwwlrn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrnozlrw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gmchpqnco.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefrssjvb.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gftomvmig.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmalmjpi.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpieizjje.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gpvmokgvq.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/ghmwkaffy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdoolpux.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gzestenlk.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhlztrsv.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmpdnvej.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gubobnlzr.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gmmizfazz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjjwvhgy.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/giqbexrqh.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxinfzzth.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gamkykiqs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gmcvcasfy.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gphxqziwp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwomswngs.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gvmthwmtu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgxzqwhi.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gblkgqxva.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyinsqety.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gigubludf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbrgwrpw.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlqtxbzr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/goawnrrse.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrtiiinq.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gzesqdrvg.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gpylyyfkf.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwoyihod.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqwegpvf.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsehjrmmx.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gklauewla.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/grjxzoxlk.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkosnmrhh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/glxxhhxhe.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gafmhopjf.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkxujnps.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gkknggxws.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhxcngmh.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/grhdofmza.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/grrjpibbm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghvcbfmxf.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibkydckd.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/giaosmmhc.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkuwziht.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyfhyeit.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjowkrrah.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggxnkoknr.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gsxvthksz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gajebbnpg.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnhxehft.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gpgvivieo.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gquisbchh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsvkoimq.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlreayln.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkhvwvzg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/grpluzqpc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gotyowoxt.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/guazhkngr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/grokespju.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmmecnss.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcfsxnyv.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlwwobrx.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gwldavshx.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gntzbskyq.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gtnmovsei.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/geioejpoy.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gptlzfcwt.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnpeerwh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqfikdhx.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnueklzni.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdqiunzq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegfnmalg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwzakdyfn.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/glrqlzjhb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gpwyljmzg.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/giwwqeztu.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtxhedrp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gesnwjjtg.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gxgohsgvw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyuaxdtv.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gliphysnm.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpvzuwwh.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gtrxyqhpc.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gesjtvvgi.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/guepynjyg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjowvwht.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gbcrrauoe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjbwufbh.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/glmcljmds.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gpvnlnfbe.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gmpwozeux.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvfchcvt.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiytlvut.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gummehxxc.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gftpayszy.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gqynggthz.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuedfwfv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gcnwlqwlt.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gzugmrspj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gsasovhuo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpkovnap.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gocdzidev.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemktfxso.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gngpwvmrq.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnfuyeoh.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdcdwkpp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gmrzjhxly.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuuiiidi.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gtmlpeesh.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlzqumki.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gyfmopzuo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrustyjx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/glfufbssh.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gpjvgpsnb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcbioooe.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gsuyohnir.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gxjejascd.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtzwhbdd.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gbuzvkrvz.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmuhafypr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrdmligy.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpjtwlql.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdebxutxw.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gboweurka.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gadunkgkt.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchmizxka.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfigljncg.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkcozbms.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gfxrkxthg.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gruqerjmw.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glshoqetp.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfjcaedc.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtstuocwx.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gtzgjngnv.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gpuwcjwik.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxkoqptv.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/grrvysxvd.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwdybvkm.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxfiedyx.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/ggtpqvrqt.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwydjdcpf.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gkormqkwo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gldcrsbpu.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxslaqsuj.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaemzpmi.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gmemfjyzv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gguodmlvg.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gumhtsapx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gnjkrmisg.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqxlhjxs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/ggxtkoemq.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gllwjhvnp.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gemzokson.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gqxwoytaa.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlrnucaf.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gfhgtmcgw.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gniwlzesk.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfkxslgi.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gnqogugex.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfveapwu.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbksdvvk.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gifaueory.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gxcrykvff.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gornmjebr.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktxnomwb.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grrethdud.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/grjlchcss.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjscugtvi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gzzhsgbjm.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/guwmwizpc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbtugzkg.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godwrdwar.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpgcfidi.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpneegmfa.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gbemapips.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gmcwwzzwo.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/ggydrokpz.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqajfynhn.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gqqrfqolt.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybmglzuj.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtymgvpeh.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/grqecruru.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoxfrtjv.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gekxbqxqp.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gaymylkfw.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gjltqchlj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtulkrbtk.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrlmykvo.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gkddnzbae.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgffkitv.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrupaqmw.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gbpqlgjla.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gainqvgkl.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/gosdocwde.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsmsdhws.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgixlhgl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwctewvw.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ganfxtyae.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggujaizht.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzitrmidu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgfznhzs.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gikclanhu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/ggwtjobqv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmutikuum.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbettdlbv.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gcwejjnyj.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gqbbvtafo.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/goswnzvca.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gigkkhqoi.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gixzjgvdt.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkobdnat.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzxweivy.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gtkpyamvq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gdspnuksc.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfgqfqsl.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gsvwxerqo.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwbjyabr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvcvvwww.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoxktrig.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/ghathsaca.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gngzhthbe.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gmznromjh.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoglcvyt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gtxjxnsii.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gstumvswx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerirhcvv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjhtrpyin.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgzkpqxk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrqrfcvu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmdxivun.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqcwwios.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gdhprzrqg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvlksdzt.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gipzwhxst.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gchyjkmyq.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcpavrce.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gucbsiaxs.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gxweeyycs.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gumrvrtgh.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gybpuceaj.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gownxrvwb.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxyookzj.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gubjvxnmn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprxrbyfv.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwhsvyfx.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgplhoqx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxfywdqs.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvddtodgi.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqybrdbyj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/grfcfgtsm.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gpclsaoff.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gdatwapbc.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/grwyxkjhp.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gszxrancf.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gowigiftt.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gxbonaums.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnywfyham.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/ghanobqtk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegaxvsxu.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/ghulqyflz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/giupkyjjl.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/grohazfsb.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gcuxnzjyv.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gblkrhuit.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwiqhgev.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoqcvete.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcpyipba.sHtML


<!-- 参考信息 -->