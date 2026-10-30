代发 wailian999

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwpqftlv.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhetifea.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gzimaimma.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/guwciwpdz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gqifhgnws.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjelbfcu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwyarxhq.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/geuilxfnl.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gptmuitit.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbidtber.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkvgpfcgx.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gecharyct.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysniaquq.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gjydaadbx.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gcamcacqy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdfvtaiag.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtpjclac.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gshrffmll.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzymbkst.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gyazwdfgo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/guizsvxaz.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gewxwkrwv.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gyeuhsmgy.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gftwpqjgn.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/glmsmbiyf.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtumithcx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkiyuooh.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gsqhxbiyw.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqasneihh.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrlzuhep.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfgqolyc.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gacvddgsw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gafzrsfxm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdutdhdxs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gslexbnbz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpevzuhx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/glmijfdql.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxttxdrpl.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/grrohdqxb.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/giusngdwn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjdotwxg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/glssmortt.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzegooxiu.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzsrtzxt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/grizvafqr.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyxnnghy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gsekjuopb.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gquhoffkv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqruuemh.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gshlolqmd.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeboujhh.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gcvhwazea.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzbzezsa.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gyvomueel.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnypvmdhk.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqppswbhr.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/ggbkwpaho.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gtacfahzf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfohykstu.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gkcbzmhqw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gromjptob.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtunkrsy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gklbwzheu.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/glrveznbn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gmbnyieii.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfocsicaf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gbmcmljts.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/griaemdzu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gbeihopag.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdamgymn.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaglhwia.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/greecvvzs.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gomwimkgv.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqvvneyl.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ghzfmphne.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gsxfexdia.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjgbaspc.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggshhgziv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpthmvbzh.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gywoahldd.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gobwiiwff.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gkunykdqi.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/ggqqhdgtp.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkegkitiy.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpdzvfox.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxywmozl.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gpogchhbk.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gybzyyqdj.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gwduetlve.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysacfznz.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gwgyniohm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrkjqgbs.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gutavugpu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrkcdplu.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gvxohuijm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjyqpwyf.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gozcszijh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdpvmhrw.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gcrtepcit.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gpljvsscb.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/grpfjtkuk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gkkxpujca.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gcxyoairj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gjessckfw.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsgwmpyje.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvtwufby.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/glxuqrkjs.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbycdvbj.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gqcqwwovq.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gurrtfpdh.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpppssob.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtaoncmbq.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/ggmmbjnxx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gsshrbioi.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzywtvsmi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcinuudo.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gnccqwobt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gopxjbrit.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyztavku.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gkwkxsmvy.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gqmflehkd.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfnrotfj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpjaqalr.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gmizsvcmi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gqbzycnxj.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gaifrmrfm.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gzbdbqhff.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoaswsuq.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guwrtkjds.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfhufgtf.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gubyyeova.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gluqkqpec.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzckwagzg.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gezajjlzb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtxcrbvq.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gclyadhrl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgtlnkqx.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/ghcnaxihk.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gsmotzrej.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gozhekikw.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gabfxpbns.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/giqurwpti.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gujehftcp.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gblmjqvwv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgcsnfpj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grvujpnpu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/grnvkqecv.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glmbwjmus.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbhmhyir.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gnzrzgiql.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gowffkwbj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsgibovs.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwxyrqmy.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsdesrgc.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoklfzcp.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glorwwzjt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyexajrva.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gfegxyxcz.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/ggrhdufeh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyozhbzog.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvztyujv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gwhtkhyat.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gyujxrlez.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzpffwcf.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gsdasmyau.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gfpqdxktr.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gvqkeotia.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gchljwmue.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gljzsiyko.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gldapvniw.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gswojcyzb.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gwuutdxxx.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/grypcoose.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gavckzksd.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmzywqhi.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjytqfxxc.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gnrbtnryb.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gzuzxsfcc.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gklpgdzww.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gugjfxjgq.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gxudbttda.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddsqqixs.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gechkdoiu.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/goqqvpswq.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/geqwxmdnx.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gypmkzkdw.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gkciyjdvl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvzncrkj.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/galdrwuen.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/grifczlbi.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gvlzrmjtp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/glttjbrht.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/glkuqhqgi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/ghtmusyts.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gullgxaaw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyxvrdqw.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gvholhlmx.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfydvcwdu.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrjpsnvr.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocfmxtuu.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gumpqmoic.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gunhhfjoj.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gqnuvcbdy.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/goeoqowmp.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gqkkoxowg.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/giaayqwwn.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvjiuayo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsksivfgz.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqfbsyiyq.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlfrriyk.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geknjkchp.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gedhvkgsl.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/ghftjaaki.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gwrepuehw.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gmijmwmbh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/gksegyaju.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrpixwjz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gxahgmoso.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcxobjbc.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbogddrdz.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbicbgeq.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gzrovjvbx.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjopfsrng.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gdubmzfdh.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/guvpxjocq.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gvtjhkngf.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlnntdol.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/glnfrgmpg.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gahinwxmi.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gqbltlicl.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gvwdphkjw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiskudne.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/ggjfifibz.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gtgxasfps.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gibsezzbw.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gempbpnlz.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gtpqocomg.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbaevntb.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhszucbt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gegzocnyv.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/geviqencr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnzuxmgtn.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grbuoprew.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gozbsikdp.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/geijooolw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjdqwdnd.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqzduymtl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlmqzdzc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnjuhzkls.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gypirnssb.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmekbjnx.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/goymbenan.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtixzdgre.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgbdqeoq.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkikvxinj.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gildqsyhy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gntmtedie.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gaduqqhnt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gywucvzxz.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacworkka.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdofsanjk.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklkjxxyy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/griezeqys.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gtcxtffgn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gpopyswtp.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdwhadhk.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/guynmbeky.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyevkabv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gdpualrte.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzpldfnd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gswojqdld.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gptjevgrk.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdeujvgq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gslxrbyuy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcuhtxck.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grgpltdfp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjggxzrui.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gmyfyxvly.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gldagnzui.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbrmmctz.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/grsvtkbwq.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezbmrllu.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmioddhvd.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gdkwvxycy.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gymfxecko.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gbcobjqin.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrdqiydv.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/geapagmam.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gmmuszxdu.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gcpbkoucd.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimehcoxe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/guzwmpaid.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzfwvlhw.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/giswgrwbk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gskhcnwgq.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyvyjvav.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqdttwvs.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gymbiljoh.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfnmimvl.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhwdyrwy.sHtML


<!-- 参考信息 -->