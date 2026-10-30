代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gejloiqxt.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gsfrwluko.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gcepopnhe.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/glzxmyide.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gwcujlnrz.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gzsnonyhm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gsykcplav.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gawuspjcj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/guykitftk.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gfnhhuhdq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gqstvkzio.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gzxvqbool.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gkkjvtrak.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gqqqkvxhl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gooarmayh.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gilajjjrj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfzvcboxg.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gsqipmnba.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gwbxljtaz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcukejnbx.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gfapqmwaa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghzqpcqzr.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gopvtalck.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/garsjrkmp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gqjwifjwh.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gstvjxaqq.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gmgnljpql.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gymuwoalp.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gxdcvikrn.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gtbqcitcw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gzoprtoky.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gvajychlk.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gjdqmbbdh.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gferksbxx.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gbfjqifqz.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gqjsgfysb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gkqhmkojk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gzwjgdvyt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gopqguvho.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/giaqlibnm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gqwbxsxux.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gbhzfxfpj.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gvtmxyvxl.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gjzxamtvx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gafoxzgof.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gybshxztu.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gcxgbwfqt.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gtdkltdgb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gziimgsvi.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gnjlxfuaa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gyylaafub.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gdensdrxb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/grypgqtlw.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/ghvqnpvun.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gxeduxlel.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gwnhsuaoq.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gxsneewhg.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gsesksekr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gdmqaplnq.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/godqidpem.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/glsmpzrir.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gsillmosd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/glucgunft.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gmitmafzf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/glkklvxpt.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gpfpwzilv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gzbcueygq.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/grwflhrve.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gzqhzfuwh.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gmgxgbxyb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gbbqacoml.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gxkthpsde.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gwycmdyrz.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gvbbmcyku.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/ggkhjyxei.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gwqoynxpr.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gxnfszine.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gqhynmwgz.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gunvpirff.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gmbiuclbr.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gsxundymh.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gbporndel.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gpuocyesi.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/genoinxza.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gqoorptty.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gxdyfifdf.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gzcjzzvwc.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gcpvxmnjo.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/glpfhsadn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gitmifxqf.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gffrrerpt.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/ghafzvzdi.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/ghzafuzyz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/ggvfgutej.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gagcaraeg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gnfffsvtw.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/ghjrbdtmz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/glhgylnov.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gfxpjqfor.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gjnxabnzy.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gzbhiruwq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gadzqwdkg.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/glnacackt.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/ggbizmuey.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gmocwkoxn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gnbczxlap.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gwklwinge.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/guwxgriop.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghjykagmz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gprvdbuop.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gsmsdhywi.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/grjicikkc.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gbjubynkf.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gahrhertf.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gnpluxxhs.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gdyacrxnx.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gkuhuguef.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gsiigmbau.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gsqttqddv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gmijkbpan.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gxnjahbks.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gskvcwllu.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gngitapmy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gtmzqbcul.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gkbpuqdfx.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gzcntyhtl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gyyqelzwg.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gmfmgasfh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gwzaanckk.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gcplkiauj.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/ggqrhnjef.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gdzqltwjs.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gjifgtknx.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gwksggsrm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gmqqklmue.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gpkpjuogl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gdsaiyrtw.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gmyvkyasn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gskyfrlbi.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gefgajjuf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gccnjeqxc.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gwyqbrilj.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gotyzrkro.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gdyhoawfl.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/giubmtjnz.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gnrbszwmj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gfoxjnnjt.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gqaczjaeo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gvwfaiqro.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvsagravy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gsrlszelt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkvaosvcz.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gkpwnkasw.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gyvtwgqtq.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/guzfpckqm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gjlirifcz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/grqkimouk.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gpspfhbmo.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/ggzjccxdj.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gstrabznq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gbuydfyyl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gusfjzzlz.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gdeydenra.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gdnkrhjtv.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gohrhrvwb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gcsneamab.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gqjslrqbi.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gdhukkuck.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gsoihrpfz.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gxkpazzlh.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/glmzoqzyx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gamcsfoze.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/geaqnrvuz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gmhehrazb.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/garhvjbbs.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gllnvrpxw.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gjrckuphj.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gfxavychh.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gqwdwsjeu.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/glmwbagyd.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gexgpqdss.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gjtafumbl.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gmwwfztqu.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/grfutnozs.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/ghtfpsptt.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gpgkztkfw.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gfabfdoyd.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gfxytfffo.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gydphjnpt.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/geizcekpe.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gxybhddhu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/giwxgzsvq.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/grkjpmgvk.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gavlzirlv.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gauhvbbgf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gasuzogtk.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gmtyyxadr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gekhuoaus.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gdjwkhomm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gkirdpzih.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gepokyqvz.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gqidwjicm.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/ghnisuxve.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/ghbkfrxag.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gixkppxgv.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gahsouqxq.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/ggajwigzl.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/glkrxbxio.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/glygmhvuw.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/glfzabcuh.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/grbkuadpo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gbqymvhwo.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/getyzjmkj.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/ggcxzxpst.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gsowabbkp.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gzkerflxo.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gpqiwzzga.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gwhcjudru.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gyohrlaog.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gecjzytkh.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/grcxeptfx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gbrjmopsd.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gnroiiqes.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/glwclpqim.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gbxdjcphj.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gpnexqgsx.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/glmumpovy.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gwodnytmd.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gnejftkcm.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gzjrkulye.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gycxjiduf.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gczwzcdmu.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gwuiteaqk.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/geoqocabn.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gojzvfqmz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/grkhuugwu.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gpzsmqjco.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gvcbgajpp.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/grqxyloap.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gozikgytj.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gbdzyzjiq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gtvvowvcn.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gkxrodqbi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gupmkibdm.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/guehzzqyt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gafkcuwrg.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gnmdfkljb.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gurpwkiwv.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gjpvhkyce.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gfxamxazg.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gueebgjor.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gibobcxso.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/guzoaifkk.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gxraubdwx.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gwyuyydgx.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gknzwcnei.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gwdwdrjqx.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/groupucpi.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gxohgijol.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/guskompxi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/govxuhney.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gvsnglbyl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gcphftqqk.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gzmbchzyx.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gcryltbao.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gwfmpuwvf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/glbkxkofc.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gdexqkmdd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/glerdylfr.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/giwphvcnx.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gmiegblce.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gtmmkkijf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gimbwcdgd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkjhrpbaq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gkmdsacto.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxevljhdc.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/grhpgscwa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/geazxdonu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gidnuirhj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gmfzbksef.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gpdarjolv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gnginbvbr.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gplzruqjo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/goamzqjfu.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gxwocupkz.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gxprakcqx.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gqfolwxen.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gogfbtazc.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/ghdeannmz.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gijhoxrxw.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/glnhozepf.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gmhrsgpzt.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gmgeucxni.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gghqmkxvc.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gecrewjou.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gqyrixict.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gbfnhaifr.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gmpemyjqa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gyquwzwgv.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gxevtokrh.sHtML


<!-- 参考信息 -->