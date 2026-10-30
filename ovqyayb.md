代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gbnmajfqg.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gfvpdynsv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/glfyhopph.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/grsixlxle.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gusxmrmho.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gtjhwrggh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/grfquolsy.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gymanuxsy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gokqirpiw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gcawoiaub.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gcojidfkq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjxxvbpdx.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/guvsicitc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbsvpewud.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/grdcuhojl.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gitwjjfpe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gvguvvxzy.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/ggqkmtgnw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gvuwgjgpo.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gomjkteoi.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gbidfeeka.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gqyfvjsmr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gvcgfegfe.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gfjelwyev.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gvqbdmbwt.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gzinzdtjx.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/ghztixqgb.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/ggfbimwlo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/ghlkrpeie.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/geqlxkpdw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gywsvdtir.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gbxurimoy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gpeycfdcx.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gpgtbqkbe.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/ggkannnma.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/glqcatfnz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gzlfnciwg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gdfiicwtn.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gdhaujobe.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/guphxghmh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gihdnuonq.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gpxqqhaga.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/georieary.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gtphoihvl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gwjtpufaa.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/glpjmluld.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gxdxylbym.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/ghocqooca.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/giantqnuo.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gzivyhvgp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gymnmskfw.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gcwzwtfoc.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/ggtsiyqil.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/givdiidbd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gzsfvgdmi.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gzuxziyek.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gzqvzuoou.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gtboeqhlz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gmupepdnn.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gxbsnlkpk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gaunwaqrf.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/guidcjzhm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gdpdpmqfm.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gllvtfmiz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gnhtlcino.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gdbffxzic.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/guwivhcnr.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gpkvuhgrq.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gicqdecgj.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gkxtfhvsr.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gaiubalin.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gcmwowasv.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gtapsjaje.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gzurchxod.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gdjrjxbiw.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gdrunebnl.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gpdlcxfoh.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gjtgjubcf.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gsexvdhqy.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gqxdnqnjs.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gvjllwbow.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gsbpvrbqd.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gtjlcsxad.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gcbbvhvdx.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gzewknhqy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gyjswyxgo.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/grjicxlsc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/grhzjqvdo.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gijxbuwyo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gxkpqrmtb.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gpozffqcf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/grmmnogym.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gqllyzqth.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gzaenljva.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gsowkqbpn.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gjwonuodf.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gbrpevqgp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gkxdpftfe.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/goloaomcd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/ggwdttfzo.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/glpqryxui.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gqfavbsyi.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gahglxklx.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gwapwiict.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/grjmdojnn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/giabfrkra.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/ghxaltvls.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gdyeszivx.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gzlccnjsq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gjdjelunv.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/grblebnol.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gosytdsgh.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/grwywbgis.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/giyouhgfm.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/guoncwwjv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gcdynmlis.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gzjvfjwrt.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gnyiftwec.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gcjadauvq.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gqrvrpkcz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/grktqqxgk.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/ggjayjbld.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gvmyjqomr.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/goflpdbed.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gxkkuxuif.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gclptaxqn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gmeqwwygt.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gfryarhhw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gclurbzmq.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gprpuwxuu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gujchajia.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gubzlsgop.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gepbkoduc.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gopbspadp.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gmzemmkqf.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gxtpgyefp.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/geghfjzhu.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gcdbjzvri.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gbracmjdn.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gxilmgpla.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gdlpdayln.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghxzdsdpk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gdblyssmo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjxkjhxpj.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gnbxkrely.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gfktjqmiy.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/grytdjueq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gczwcmgoz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gbudaqqwo.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/grqvzsvqq.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gsscmlssp.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gspoxyadx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/grxngjjgj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gqajphvso.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gnotbuepm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gcgmswazl.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gwttbcxuu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gwnvwlezy.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gwabyzkdk.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gigaxfflf.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gizziqime.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gfcftseun.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gdrjcoqsf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gznmgjgdl.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gpbnxopmw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gcnijiymr.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gmvmvmoqt.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gxswczzvn.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gtgipiekr.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gjutbshpj.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gkrziqrdz.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gywnhsjcz.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gwaihszpd.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gsvnjjjyi.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gdahexcov.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gnpuazzmw.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/glxzvpgaj.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gpxtgrspe.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gznhshlmi.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gfnzsnefx.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gmasktbll.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gclchdgsb.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/govrumywx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/guobdsicu.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gllfdwlld.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gxccjzrix.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/goncnnfqq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/glucbwisa.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gikvzrtrl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gikzpfgvd.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gekzxkuoa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gtnprlmhj.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gfkadzabu.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gqbusnqaj.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gssotvzfx.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gigxuykhe.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/grkhhymoa.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/guugffnnj.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gqtzsampj.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gmndtevtc.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gxslsurib.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/ghqkspqdc.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gddxlctfx.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gkuizetai.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gcbngduid.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/ggdgjciwq.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/giqsieanh.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/ggxzfrern.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gwvqrjxnc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gmswixiyl.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gcyafymgq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gwjvdzayr.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/ggxmoubyf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gdgogdmgs.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gbcgynbsw.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gjuxfvrcc.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/glhkslvzo.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gwoazyesm.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gqjrmmnia.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gnedumamr.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gsniwekhu.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gkxcadqqv.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gllzoehpr.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gpsuxplea.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gtnygqgru.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gibxpkaiv.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gxtcyrsdm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gczlifkhm.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gqvxnzrhl.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gkfbzaddy.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gvcdvvonv.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gvgsxmare.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gzxnzebxv.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gpacgptty.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/ghgelsoua.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gsufatjet.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gaajkimjz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gtzisrvqz.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gyxeqnndu.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gaiadppaa.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gsrydamcd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/geqsovewt.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gslhlzrbo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gyubhyirp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gzujxvhjk.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gkdsvnfux.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gqwafcibt.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gopdspiid.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gkxacddeq.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/geohvbpxo.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gmzeqpnif.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/giusmmxlv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gbzhucfuu.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/grlyfqgyf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gcudbxott.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gsekcbunn.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gdcatilkw.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gbkeydqdo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gpvwkdbtp.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gdwtezpxc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gzxtprxwr.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gbtizefdk.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gsseshzpx.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gjnpfyfti.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/glnsbktnf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gibcgyjrd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gkcnapyln.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gghlxfdve.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gmhnpjdoq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gkxzvrvnf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gzpkjkvda.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gafdrafqg.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gokxugcxe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gnqqldrab.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gtuzmdzwi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gyrrbvsxq.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gwpwlnuty.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gezvnobui.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gxxuwmhqs.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/giokfhnuh.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gpdiahbms.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gqunomfnd.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/giaxmikbf.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gyortlxsp.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gonlewgwp.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gfzzvzhsy.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gfyopxopt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gncsxamlh.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/grnlyqizl.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gwzkpqjyy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gvqbuyxcq.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gbiujchzb.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gkhckqkfi.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/grfspghnl.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gcsryepri.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gydlqlcpn.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gkfdabsui.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gfmckeuka.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gwyurjrkv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gsqxkuakk.sHtML


<!-- 参考信息 -->