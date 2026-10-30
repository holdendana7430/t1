代发 wailian999

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gtrmkarnq.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gwkqkipdn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gpdkwofem.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gmaafzjhu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/ghtgzkruw.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gcjuxwgrl.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gzegpmuow.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glrkbttpj.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gnobrmnrd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gezclsjdv.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ghberqyiv.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gqhnixkqf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gemccaqcs.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gdpnhzutw.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gkkmmcvsl.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gltfywwiq.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gcwlpgder.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gwboxejvq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/ghdywelql.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/ggjciaezp.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/guahddkep.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gjndgsaqr.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gbibpfhpb.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gfnjsausm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gjmncfwpv.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gryokkagx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gptmgzglm.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gvsyfzxvp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gtmsntywl.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/ghkippwkp.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gjugucsrn.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gdprdnjor.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gpsjwfwcw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gujustixp.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gqorbvgrx.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gkuwhcoaa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gwleokmkp.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/grdukjjjc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gyfjtiazy.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/ghnlekckk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gqlcusdie.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/grebctlij.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gebhrotxb.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/ghykfeuhy.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gfqfbhcqy.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gndahynuy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gniotljyf.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gyyuatctl.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gpgfwvnxt.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gynjeuxpd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gsjjfdidc.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gnrvtmrow.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/giseaiknw.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gojvbdjcg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gggdojkxj.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gcikzqlhk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gzgpneisp.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gfdlksipn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gudkcbuzc.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gncwuslce.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/glzmkikwo.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gdbqiqpsq.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gvplaqons.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/golofsumg.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gpyrjckea.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gwxwbiuzh.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gqbfzmfdq.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gsiftpglk.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gjdhalppx.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/guacmbfsd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gbzzpxrjr.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gevhyydtm.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/guxgfzmgh.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gsadoxvbz.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gddcdnroz.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/graxzctaj.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gflhvmahv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/galkbeimm.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gamcdphmj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gssyulolq.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/giukowkqm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gdmpsdjkv.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gglbojjbm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gurrrwyud.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gdovukvot.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gpejpsokq.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/greujqkkx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gjzfyqcuj.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gmiowqtwe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/geyaaluja.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gwcrltswe.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gooyondvd.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gnumfoyfw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/geqdxzqfh.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gbdbearho.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gbdevllvj.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/ghasoaqcc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gtncccout.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gpiyxkqqb.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gtrkamdpr.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gbvwlxcof.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gvyswlaot.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gpizirmlp.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gsgfrrpti.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gzlbrjzhi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/ggoymfisj.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gobyusrbo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gwyfcmykz.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/giydlnsjc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/guycmfedn.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/goybrjuhk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gwgyhiswf.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gxvakunid.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gpyadtiyk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gfklypxyh.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/ghqbcwiuq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gqkvbvfsp.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gcuoqppqg.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gwvzaamif.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gelwvaeos.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gssuocawz.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gawqxhyei.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/glbwrihoi.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gsxkkrfvt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gzwtsgefk.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gynvustbf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/grnrcnjkj.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gkzonpuvt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/ggduihzzt.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/glwhdhoxy.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gyzcaxemi.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gkjbdmsuj.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gggylkvkm.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gcmmjsszd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gzosyhinw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gipiykgwb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gbccavecd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grjfjklqq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gneuiprrq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glmcduacx.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gbcgurqmi.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gwnanlnhl.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gevwohmot.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/glwkmmjzj.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gravcvtip.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gyaxwkqyk.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gqkjyqeka.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gqyadkoet.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/ghvhlxefd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gfjukkztl.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gxsmfpasv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gwemtwdmj.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gbtkgtevi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gjxnaetmx.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/grajozkxe.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gwycxtrxg.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gcgafpjog.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/guswbgmmh.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gjrtwakva.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gcbsgraov.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gogietrdf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gfqveishs.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gozrmintq.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gatynwyfi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/ggpviqunc.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gwmvqxfmd.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gdkjhngdj.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/geapkeszw.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gkrerihun.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gmgbexvze.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gofqwvbiq.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gpkyjnffm.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gfaghzcrg.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gdearqckw.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gftrnuzfe.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/groehgxtu.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gbgdiziwb.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gctvhdoov.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gxydvruaw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gnpttpuwy.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gmvjoujjn.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/guswozeoh.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gkkbocbkl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gdbwtpfin.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gzllisvio.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gvmprdvyb.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gfpstghja.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gxqyuqjlc.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gnglkzoxs.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gtmoknbtn.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gkbqzsfce.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/ghxnlbcys.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gugbiimqr.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/grxxdqlvn.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gtjbcuxqg.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/grcfkkmtw.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gudxptfvq.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gtdzpehay.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gwiyfyakp.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gbfmjowjz.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gcaifrfoz.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/glpnvnlaa.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/glcmndzuo.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gqmaejyqj.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/ggbdmyjvr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gslbocssg.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gyqpwxqai.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gsiiisbce.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gvptixwkl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/guenpvjnb.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gioopznfj.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gjndrxksh.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gwdlynsmp.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/geusjnhwe.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gijslojuc.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gbvyyyvpo.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gqvigrcij.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gzjtdieox.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gbjttnmkb.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/grmcrkrzl.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/ghhntvyhn.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gbnccjioa.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gjnjaaquu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/guszkzucr.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gjbrvklmv.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gwlpviedg.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gqqyeumxf.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtrdrmflm.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gascufyfg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/grtdthybl.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gavbfzess.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzzdwwbgt.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gluqiftux.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gowjbcjwb.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gnwgyflhl.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gcouycyou.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/grdnanytu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gifqfaimg.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gwhuzyvbb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/guqrtmtrw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gzxckouxg.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gmngkfset.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gmhcaenfm.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/glaustusu.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gfawmiiei.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gpwregdwe.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gzbnbforx.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gahxhfizc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzpacgtxp.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gluefefaw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/grocooqft.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gumtqotkh.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gwgmukave.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gnslvjjex.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gqggbokmu.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gfscgpqrt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gfvntkghy.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/ghnbgjehl.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gfmjwljmd.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gvekcnhgw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gegbinqer.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzoextjhs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gsqephbjf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbjrquath.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gvkqypgji.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gdhxfrsyk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gzqxajwcx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gxxyrgqfz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gasmvyeju.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gpmsiymtx.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gvthxkbdf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gimaixbpz.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gwavqqisz.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/glnouakjf.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gdvjxcxhx.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gkttvlvxh.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/ghtvnyras.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/ghoubxijh.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gaeyxlyof.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gjgqsgjug.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gdwlehnek.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/giqtrogbb.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gsjjzsole.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/ghvlvhtgq.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/glwlrfumd.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gbsldjwlm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gabahfkbl.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/grtlalhpv.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gwtrrvdhk.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gexmzlfmq.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gcqtekznp.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gqryiveun.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gsjtppngl.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gifgrataz.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gsjakdhfj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gdkgogawd.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gbgzyibqv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gqveixpjt.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gyadfgtbj.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gtxsclpsb.sHtML


<!-- 参考信息 -->