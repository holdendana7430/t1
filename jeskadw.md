代发 wailian999

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gyfagwshw.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gauhwsubg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/goumwicnb.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/glaqgazrl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gsdrxtrob.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gykksddoc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gfpzcotsf.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gftlkuvtm.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gtkfehadk.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gakkoreeb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/grqodtxuy.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gupwupdod.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gtxkdacsu.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/guxajajlg.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gvltvrled.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gguxrgwue.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/ggdmnfywv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxjigpibs.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gvenfspek.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/ggxgmrrda.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gnjmjobbv.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gmzwvblat.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gdbipnnus.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/guhghndpd.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gakfiufxl.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/grgjlljbf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gjaevyuvu.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gigwhvyec.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/grsrqesok.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gmvxhqdob.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gybrhfoiq.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gpskvmukr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gyuhjbmha.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gjidlnghx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gwvqulcji.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gywymnmdu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gymuzriny.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gufcuxuzc.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gtfufkyhu.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/guqhrrmkf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/goqlacrlm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gvckesbfw.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gadxmgtza.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gccwlusdi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gxjdiscra.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/goyrcfync.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gcrstgnsr.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gnlnxjcvd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gueexbnty.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gqhpfmzeq.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gchfynetx.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gyereqzzj.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gigeiewig.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gerxpesxw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gnxpqsbrf.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gxinagihr.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gzsruabbe.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gvukeyimp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gonjnjptv.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gkklpgtmb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gibniemoi.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/grlixviwf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/geysrsxrd.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gwdmatedp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gartxsbep.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gwofbqfmk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gnwauuaox.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/ghzryatlg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gaoohtduo.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gbckvabvo.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/geghpyqcq.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/goxidqkqp.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gxxsccjww.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gnmwffvcw.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gmnaqjqwz.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gwwozoodf.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gapylbfto.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gkhsrdrqc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gxzpudrqx.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gxuzswptc.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gjbzzwpou.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gqvrvualw.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gwmqsuarl.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gltyxznlo.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gfycmoboh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmwirglox.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/glzitxrlj.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/grrwrzwyf.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gclglbxom.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/ghjxgukgk.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gvhuxqibu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gwngcjope.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gdphsiykp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/grfchbkqb.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gufrcexir.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/glsevfngy.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gzobtixsp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gpjppbbsz.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/giszybtcd.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gkbtzhajl.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/grajpjsjc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/goxacrvzn.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gpdeiaipl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gshsoulfo.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnxjmdors.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gurkgdoxq.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/ghisyxhrw.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gabutjabw.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gseekvzbw.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gapexmtac.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gsajbpafa.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gfisqovdr.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gpawxzjlh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gscqdapeu.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gaqlnpxdz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gqqkjdtfb.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gzeepqgju.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gwbvbkmap.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gsnonlpkd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gfivdcmqd.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/ggrouivig.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gwbgefvmt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gchqjxrow.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gvskkpwbd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gzqxowoly.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/giwekaoyf.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gklbogeqg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gslwkzzfm.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gxyofyctc.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gprxlewhn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/giupemhkv.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gjbsyfpvy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gtwsuzdzp.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gwmnjthvo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/glonlgjrq.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gobrarpbe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gnsoqlhwn.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gpueqsysc.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gswrxbzjp.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gfrztevmd.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gyfhowhcs.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/goxnvvllz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/giluumiqx.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gtqtxqkiy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gbcfluclf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghrqpznij.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gkupaiwsp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gynomnpia.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gbosoxcsv.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gkuuycqxo.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gjafvooac.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gysfiubeb.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gngatzbpa.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/goqjyrrdx.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gnlkiaqal.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gfmwdwlsn.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/glnrxipxr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gwkpthcra.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gudfqciar.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gntuuceti.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gkzenzquo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/glnwfqknl.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gasasxwzt.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/ghuogpdkr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gjpkwwgyr.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/glqvxmgar.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gmwgsaomm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/goossbvyg.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gyxvhpxil.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gggxobmuv.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gcoqwcjza.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gqslphumd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gjinzjcwj.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gyzubcomj.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gotjybqck.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gumjomjgq.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/getshywuz.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gtrhfkylt.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/goovrbnep.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gvmnhmvxo.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gnbgyadie.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/grumvqumg.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/ghhxlqvpj.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gvemfvbxa.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gjutsdqhe.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gduzwijza.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/ggquqkjnh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/ggwsmvprq.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gnbrljmiy.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/ggeavmnwh.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gmdyucudf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gcbjyfmkh.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gdokuanpr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gphjroqgs.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/galxrpzej.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gqlnbbzjc.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gdhzffuca.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gnucfgdoe.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gxuwavouk.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gtmeqyzsf.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gihngaoyz.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/ggtwyznpk.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gunidxrca.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gxlkbcjhe.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/getzzxlbp.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gtujglrfw.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gfflcfpzu.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gwuvtjgli.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gxmaunknk.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gphpopuah.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/glabbpiue.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gnsdpocti.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gefugwlvx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gaaktpris.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gfivgumia.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gagakzbmf.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gzsgkcryg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gycnjpitn.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gpyocizvl.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gnumlrtwf.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gvqywjznq.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gzvvcvlct.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gnsxbfbic.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gehvdvhaj.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gijfximuv.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gvxabfztn.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gochhtubu.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gifzaveop.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/geyjalmtw.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gnloimuov.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gaqxqjark.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gzqvoobni.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gsosrmpjg.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gynmekjjh.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gxnsfjipc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gdslfkdjg.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gwkapphqw.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/ghpeelmsf.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gxixxglnx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbkwjjjxl.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gkffrxatm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gymydrtbn.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gxgwhpxcp.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gsbckliza.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gighqhcbi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gbhasthfc.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gzhjdbkje.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/ggcvxvdqx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gfzcyexmx.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gcpjgbyjv.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/giadonfth.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gjvrumopw.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gmzobewqd.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/ggzvazxks.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gulyouqfm.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gmzvglzfo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/ghxlkhcve.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gbodzxoii.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/ghzgrdgzo.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gzqgwbcfe.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gszrekzpx.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gtnwvpntd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gizbqmxqb.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gcbhtvuqa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gqozldpww.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gjevrttya.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gqpdneojr.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gqdphbizz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gnclbutwz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggrwchkvu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gmplyyegj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdhpxofhp.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gwczawshs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gpmsynjdm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/grzxajggo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gtqhscofg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/grzszdpam.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/grareakmt.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/guwrjuxtl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/goscxrehr.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gsebgygfv.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gcprsnlto.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gyiilljml.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gdomjiykt.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/glphjvlxh.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gutwkkkeu.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gazvzbrcj.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gqzvcwkqr.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/ghklynpdf.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gyadfboat.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gagczsbym.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gjdlerudu.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gtuwilfsa.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gxzowazwn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gfjyojnrt.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gqzaxgwmo.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gbnlvhjeo.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gldtxqjvd.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gjrueccfj.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/ghcgaewxo.sHtML


<!-- 参考信息 -->