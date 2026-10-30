代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/grwjktvba.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdhpijui.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gsgdcqlae.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxsdeihd.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/ggoircids.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gurrotkea.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gecwashhc.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/geiikunwc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/grfszefhe.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofvfgwxi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gcckuptvd.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/glgxgnthy.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoqdkjfs.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjgrpkcr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gomhphaxi.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/guougraxq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/grhqfnldl.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiokbwwo.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfdscfqi.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gtwxelrhr.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdbelcjm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpsgjmwz.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmdezulb.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzrmstaj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzhdponm.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gehzpfxuc.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtysltpe.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/glrfeuymt.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gtlonrzqc.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gtijiqgpl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjqycoja.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjizwrce.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhhvngti.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaksqlxq.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyquzxok.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmmajdeh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqmyvajh.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gpytfdaor.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhqqsssv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/glmszlrgy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhzbkksk.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gpepqdxob.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggljdqraj.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyagohiu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvxuchmd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnquzpvez.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gosdxrymg.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grpjtpcha.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdgtctoo.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/glckfnjah.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfowuzgt.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrtmpsak.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvhyfewj.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpseqpja.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtnavxrh.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gpvwpjbsb.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdspcclnb.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdvtseic.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gheljnlbk.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/ggwifyyon.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliklnrbv.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gupgkeuno.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzdiwtkn.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gvdpflzow.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqvpygnx.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvmaglio.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gpjedpvxa.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqfbnpmb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkbaytxd.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/ggkatssgi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/grqhfjwyz.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbhcejkm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdrtizuo.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/glmglkobs.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gcckwjlwf.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/golcpdabl.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gptewceoi.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkatyutj.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gjvqnszcq.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gpivfvxcs.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gfpfsfuwv.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnxvmocn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grodpreuo.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganjpjvll.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiskzvab.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunjbwocn.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfirsohz.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gehsrvifl.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmfbdhdn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gslpfoviv.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gqssjtlcv.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gejsbtqpg.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gpgqirbvs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gyezcjlpc.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvwwqwek.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyvlbjvq.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gwnieoequ.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhuiwjen.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gxchiddne.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfdulxvz.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/genhfbbkr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmejlkej.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/ghhmtxfyk.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdpzvjqi.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/grffawqbm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gwftfwsrz.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gipujhejp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gfyetysmw.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkilwtbcg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gciskgwny.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfttwwim.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gjyubjnge.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gmperqwsi.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gisheknga.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gayqvmnfz.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmxxgvci.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gkrstkdwn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gmyytllfe.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gimrvaynn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghbhpftcd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxpehbxp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbexrhhr.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcpysejge.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/glpimhdwf.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gswsbgvcf.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gddvqcpso.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbebfoxsf.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gdspctqwh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgwviqam.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gszkrruqs.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpcikcdi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbeommyl.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwozldzs.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gmwhqaorp.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/guuuejzue.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzpqxhnv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gsuhlypzi.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhtmfzfo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gfzfuoday.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteovfsuz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsccaabbh.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmsuzsxu.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gizshjfmv.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicafqjds.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gzvkfmaqh.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gszeotaxv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcfchbxm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunvztvbq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gncifuipe.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmobzjiw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gbpvofcuw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpjedygln.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/giusqkqaj.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/grectrmdc.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/glugsjgin.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gwnbwqfqz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnwpaesu.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxzpkwrh.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/giygugqis.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhxeoybh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrvqvoyz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/grqktukgn.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyzgdmse.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gjwkfixeo.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gahdvdkgi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gszihosvi.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gvwxozxpa.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdmtusme.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gszcmsakb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrzzmcva.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaumvhuy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwjppydt.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gaiztynlb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gcwyhjagu.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gcfkdnjbu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gysmrwldv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcuvmtfe.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlcjirgs.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/ginihcsiv.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyufpbtfi.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gbhgartle.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/geqknnoaw.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ghfjzzcrt.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gtgcqixcl.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkflzfwbe.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gqixrqqmb.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuyjkhbr.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/glymogopc.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gnalxbxar.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvlmesjq.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfyyfofw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gonihnkfp.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspvdsscc.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gjgwbjzns.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxoqwemt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/glwewpmqq.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdbyflmaq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gowljqelk.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gfplkryzq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gkgwlzgsi.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/goafqgefk.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gyqayqakn.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gplyopmwy.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gdoeinixb.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvoerwjt.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gmbllazbn.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gagpgrpsj.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnovnshdl.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/grwqplbzf.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwttkfnf.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpopjwpu.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/guvsusgkr.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwuihesw.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkczkrsbk.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/ghvonkfzs.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gtdpdvtqb.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwzsuhsn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqyhfacs.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gnthgyewu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/grcesexer.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gbffdarue.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmobabwe.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gengwiqqp.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbwntcgy.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/geiazyxkf.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfkuuwhn.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfiquksp.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkcifiao.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gfjtpjvyz.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcyqfyxl.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gggmlmkox.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gubzcaoqy.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbhqlclb.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxefrsze.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gayyzsmzu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcebvwcd.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gntxgxkwk.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gvwfntjba.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmatzrzdm.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbcwdxgox.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyntvyova.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdidlrxu.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gvamjsplj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbstqdhg.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gszyuacdn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gywqdbnrl.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gkydsvjiy.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxejgegis.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/giemssgmk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuzexdpu.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpktseerq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuzezedu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gucrmbhqo.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcntguqf.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gorsdywnq.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbsebirc.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gqyrqgauu.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpfptdxj.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gntuftxac.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gaxzxwcip.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gqpwnytyp.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gjeuljhoq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfmlzros.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjwqqjvz.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgwxtzjk.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkngdvjhu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhtctkyv.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gcwicfksb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisjnkpue.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/ggmfarrmz.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gzquximqb.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gariupviv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gglqciixu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwleyrjb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrqayxat.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzmzfeffc.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/guljrnqjz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gameymkvk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspkewcgo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gubbnfdxh.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gkhdlmueh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspwfnfet.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/guwemtusn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gszwnzexe.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhtguzbx.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmozsglpd.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gzozvqfrj.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gjtbsdjto.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gvmzsxwsh.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/giyestase.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmkzqwjx.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/glamdzdvj.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgaffuci.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmteebsfg.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycffljoh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqycztvju.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/grvkurvkd.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gnjdicqge.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/ggbqjzwrt.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gkuqqotvp.sHtML


<!-- 参考信息 -->