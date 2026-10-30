代发 wailian999

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gaulkhbrn.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgmhoxlx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyexsunko.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/govtboted.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gizetlxux.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghebalnpo.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gfwzcldur.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guttqgpxc.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/goemgnfjs.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grrpdgdnb.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gtdqgvfsa.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gvqhigyvl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtmddlzu.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/grjuysqlc.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gkhpalqpm.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gfqpzaoiu.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafmlowsy.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/ggbbdojzk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhynghiu.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gcgwbuqcg.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmovahdde.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gqqztazpm.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gzkqdkrli.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprklmyls.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbbuelzg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/grgdvttak.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gmcvqmclq.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gwrnygkwk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/grisfmqwf.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkxjlphu.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gghdggcrp.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntltupso.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrcjngnu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpyamsyd.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnlfyjnh.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqodmthwn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggymfzbof.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gsthhzvet.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gfgmpjnpp.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gpcdjbncn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggntvjnmo.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gscyaowmf.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gsvvlvnpz.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gqujdbivh.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gcvlisblo.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ggniyvawv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaqqirnu.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/geihootcd.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gwjewbrcu.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gplitmubq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcveuccin.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/grfkrqnai.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfcxvbzr.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gnpscjqjx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/geigdgssz.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfpfeqyu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/grwznfkfj.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gqrobxpmv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gpuzzbetm.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gshjaycyi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gpyldancz.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlwbaxwe.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gjhbewzoi.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gquzzfbss.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqovzyvj.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gwhhkzqsk.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmgvnmys.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/goglkkgju.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gfjjtuwyx.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gybwxzuzp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjspwdbg.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gxflpzclp.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geziprpgs.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gjegddeuy.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gejpwtqxm.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyhiirrr.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gnkweynjz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfujjdwwi.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnwqgkmy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqkziitd.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/goknhljzf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gllorhlni.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gmubhpglk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gytahxnye.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gchlqqqcj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgyyfwky.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvlwtfnn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gifdzdqtg.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwthvwyr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gokcdlapo.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfyritql.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpdghlqg.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/guiduoybn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gxirzinjm.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gmulgvyxa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gixbtsuee.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibkrpehr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvbwpusm.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gggutzhnc.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gltbcjqrs.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gbabeigwf.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/ggmuensls.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gxorfxsrw.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpoytjacr.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnszjgwjy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcosgyeqr.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gzzenvqrz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/giushjpal.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glakkndnt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbamuxmhq.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqcvpyyft.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjeyckujf.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gndnbzxcz.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gefgmotna.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/guhrxcmst.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/grgahdnew.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/ghwjiqhqc.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwyisgjg.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyhlhnml.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjwkfbuo.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gucyyajzg.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gmgbthrwi.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gevbzvega.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gmldkddqh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlzoqopv.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gwqwasiec.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gnwbmenno.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/govdhhiuv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtnrgxmy.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhotfqrb.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmcsklgk.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gxllztqvx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyittciw.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgutlagj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrckczna.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gwpbgertx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gqifhbuhu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoowuecm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gnvkgjlzo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glrczajkz.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkzfrduk.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/glsozfgzo.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthzzatjn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gjotnklnq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gynfftmlw.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdahyxzp.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gkfpcyvpu.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfkvyzou.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gtjsbjgtn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gefbckzsd.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/glifcdcci.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gnykbhqsi.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmxmfdoh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gllhhzxhb.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczsrogjl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfazfglro.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxdlrofvb.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbibjazfu.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gnyshpidq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gudlfelqw.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjjwlsuf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdxfhgsp.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gqglowwva.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsurakhz.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaknnlwn.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gidgfiahg.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoihzikx.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxnmovvb.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnrfznet.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/geeerahym.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjplwzzm.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsurfnobk.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhbmfppa.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gmwavrrgn.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggakyqxez.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/goidzroxy.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnutpoly.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufjqxgjt.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptviiexd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnecyesj.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixpgires.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gmecnoeba.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gbriveewc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjqpzpwv.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/glanyzijs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gcwhvjkxm.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gimcwoeme.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/glczdgbtn.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazpqtjcl.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gvfkbzhdc.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/ghxsmcwie.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaahvzadd.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gndfihtmg.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtlpuewh.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjcvalka.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyfaufrq.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/glrgqrttw.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gstxqeyxt.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstujvseg.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/grotrmsnp.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gpctastps.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gewkizfaj.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxrovnrq.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlqplxns.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gyspztoyz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gqqbdfywq.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gyctoytrz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmbabymd.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/garzcyffy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjqtpegy.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzstpzxwx.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/glpgcauxu.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gafbpldhy.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgmvuqws.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjgynnvk.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gardixrzv.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrnzfspj.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gylvaiiyy.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gkabggdfn.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/guzzyfddy.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwqhalua.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/ginwnvqte.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddvxryja.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gprbobbyn.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gitttltaf.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnbrrksm.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmfekbex.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghacbzxcw.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gyrqblljj.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/giqncthxf.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/giktwwqad.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkbkjvsm.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gqsueisqu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsucahyv.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtaruxzs.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/glslwydiz.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/grqvjuxdr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohlfmbvq.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmlbftvti.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gffssywrf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfmrprtty.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxocxrpx.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoccfeld.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/guxwweiio.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gprccuoqu.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtpwnwuq.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggowkmwxn.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gyqqrkscn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gfocsqnrk.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/golzlintp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgsyxaaa.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gwigvctge.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyouyoomt.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gcbrzsgmd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gcchqxzos.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gujnxvpag.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gxgnmamse.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/grmgzbvvq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguuphmdc.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gydsggcfj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/glvekvosd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glspubnro.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/guqswqyga.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdffzchck.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/galbqahzn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gmrbqqkww.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gazyxruby.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdfepemn.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfzrhlid.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/girwobzib.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpfpuoqq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyunfyru.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosixgklu.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gncsrjyed.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gcacodwip.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/glfjgsrul.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gelqozewk.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gdswbcoxr.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggddbwvwq.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gkxagrqfd.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcivdkrn.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxaiboll.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvraolzo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfkakpgl.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gfdlaaivf.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gkhwyoobe.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/girxxjsjn.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjdrhqiv.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxjnjqpt.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gcvuorkts.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gazbktodu.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/griryqnbk.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gvikkwocr.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmucohkgd.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gxfkoljwn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuklcudm.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbdtnbdj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/gkhmtejys.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdcqilcs.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gtvktdotm.sHtML


<!-- 参考信息 -->