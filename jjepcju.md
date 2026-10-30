代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/goadukjrz.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gnrbplhrt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/ggyuycmws.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/ghaqwbtwp.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/glwgxqpkc.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gyizcvjnq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gqghtziwa.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gpuzlrtwv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gevigvwua.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gmelpqleo.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gaqhkxmth.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzzadatyc.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gqcmfwstw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdhjgquep.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gsbdgjdlm.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gnfaewirf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/grahqxeqg.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gejzfnnyw.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/givnrzzkb.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/guktfyfvp.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/ggqnandnm.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gpdkkujus.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gqbgjoltu.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gnnimayol.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gajhcrlmv.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/ggbcuqycs.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/ggmwcqjdx.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gdspkylqr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gdaylzhgt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gndorcqcz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gzugffbbi.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gzpjqjfmb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gejpfqynx.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gpuszduus.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gpxterkrl.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gbmuytwee.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gsartrvxg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gbrpwgwnc.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/ggqdiilqc.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/guozcmlzi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gzudppigu.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/giclygwny.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gramwdrsy.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gcwnkgihw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gpkkhmhes.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gbdcwyuln.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gnsanlrlj.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gxvedmepg.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/goiikklsq.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gpthtispm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gpbzohxvn.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gvlksqbsz.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gjdvvsblt.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gntujdvfe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gfncbfwke.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/goekvqvxi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gmxgrtqcd.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gsfkihiet.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gcohtqpnz.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gugxlajds.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gvucilnub.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gjdaixzde.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/goulqarbk.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/govhjkeaa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gutfjtgbs.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gisyuqoey.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/ghlxmxhzv.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gschxglmp.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gcmzfzykw.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gpydpaeqj.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gejrmwakz.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gfiouxwyf.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gjuukwsgm.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gmrczjblw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gjzeoepsj.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gqorxaevl.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/ghtzovkun.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gcwqazeqw.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gesshclxk.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gsdowdect.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gkqamxmtg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gdvcqmdvi.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gixknkgnn.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gimisldzt.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/givzwjteq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gpzfkmnui.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gbyzuyoqa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gcaueiovy.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gikodgynv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/ggfpbkuop.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gtjeqmkge.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gyzqsiqsu.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gkvogoisi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gwijddrbh.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gdelqsdvl.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gagtwvfvf.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gxherbkcv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gzlliecxk.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gtdyazhqw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gzcmocebl.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gzhersnto.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gassgftxu.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gmggfadhn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gfyzzxikb.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gbimxmplr.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gknszkdyc.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gmziwixwh.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gdrpuoebu.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gveyaocvz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/glpngekfi.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gpvqwgtpf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gkbindpdo.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/ggvtrshsk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gphudsjhg.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gkmmolyih.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gunpqjdvm.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/ggurjagcb.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/ggblikxgg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gkmtojgwi.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gndxortch.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gmfsekwjr.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gkyaugikx.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gngdpyoiu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/guqfdfelm.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gresdjull.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gfdickscj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gjriyruvt.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gurughdfx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gvpwxlqfk.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gksakwhzz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gwbscbhqo.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/grhmddwqm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/golnvqvyz.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gyeppvfrj.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gujfmpzmh.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gkmnjtgdh.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gmwxxfejj.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gewopyjtz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gewthtvuf.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gsqkmmwsr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gwditubfd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/girajntpc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gvwkkpuap.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gapgjippi.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gauqquhts.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gnexbxdgj.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gqhwybrup.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gjgdcpazp.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gtavoflsd.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gdvnwsfei.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gljunvvko.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gisrcvwie.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/glnuwjrfj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gymyvrzyk.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gqtqqldtc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gydnikawl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/guihbkpxv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gspwiexsy.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gnnjjzhpo.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gzqdlnyjs.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gomhkfwcl.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gsqhfublu.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gctoxtdzd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gixcejmgg.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gbttqzsxr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/grbemtiip.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gvgxhfptj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/glqnfqzqy.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gfboznfrp.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gggcppijw.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gycndbhpe.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gewwrbcoh.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gyjecswbu.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gcexhwurk.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gnqwmpjmb.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gzcffsmgd.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gbawcuahj.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gugqwurzn.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gurrsubxu.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gjbknivjf.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gssgjcivm.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gepjxlced.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/guownfsbn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/ggncltcja.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/guqhrpprp.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gppvyoojv.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gpmwnyctd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gefahicwu.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/guonbeuvt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gvuploadr.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/grwomrwhu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gljbdkpqj.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gwmrmaodw.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gjymjynrf.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gchhhzqui.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gcvepdmid.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gafkuwpey.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gztabqmwm.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/glqmpciah.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gznwsxxjf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gvgzxykxg.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gqvwdkafy.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gbzfricpz.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gvriwwhrh.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gxjgswcok.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gjejryhhi.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gszedwqwr.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gxfquryxo.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gglcdbexl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gdranehnv.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gxbrfugvt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gpxyiixyf.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/glktqnzxe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gsjpwgdss.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gjltcnzfd.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gauiykxzb.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gydnffwjf.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gmhgoxwug.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gfzrwtziz.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gyblrtahr.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gwjabhgqz.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gpgdnwayr.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gjjxljtfo.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gauxezhwr.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gsxsjiwqj.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gropdhquo.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gmacvxmfn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/garcjnxsn.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gxlbqekhu.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gbkrpumll.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gubstxmdl.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gnpcaahvs.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gesufzcuy.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gzbprtluw.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/grpgmfoxt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gpbeankxu.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gypepjbbc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gpiwsscih.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gmunxieeq.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gecmcwmhy.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gsaizxgvl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gunvgcouv.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gyimfgvjb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gjpnqeanf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/ghqalhgck.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gkmysqahn.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gjkuyspdb.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gesqpnzqu.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gkiulmrbt.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gwaqrigii.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gqtfksmnd.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gkzobsrkv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gfnfsooam.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gvnivqdti.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/ggfudsfbh.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gewtnagvf.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/geohcuwpw.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gwiglllyo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/ghgndtqor.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gixfxjgin.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gswuluirs.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gwvtxsgie.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gljkxipuk.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gtaunklgh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gklzvgzaa.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gobwkouol.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/grqujdjzv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghykekrjx.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/goxusbuot.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/garmhcsfk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gkagunjfk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gtneykbwn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gpmjpyrup.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gugxkpght.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gadblhtby.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/glfwdidws.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gvzubbvpo.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gmuvybjww.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gzgxfbiki.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gwknegbgn.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gjiysokpq.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gobtkqjkl.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/ghupqczbh.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gjoihfaxw.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gqwlrkjkj.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gceqbdxol.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gtgvyxgew.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gqmrxtvww.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gjmayprhj.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gwvplfbmc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/glgytybrq.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gsuhiqhbq.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/grcmumphw.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gchfymmce.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gncghohix.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gcrtrfhjg.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gbhkhcjef.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gxcrkrghi.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/guujtwpgg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gmibsxgiv.sHtML


<!-- 参考信息 -->