代发 wailian999

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gdqzktbtv.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gbjddznuw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gjwutsrcp.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gghplmzxw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gmukwfxwh.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gngamkjfb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gimzgbejd.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gjvcdugem.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gmkynsade.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/ggwxiklrz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/ggmycxjwy.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gkivcrprm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gcckxwpxa.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/grtlwivzy.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gfgltwczs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gquitickl.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gqduhmayn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqeiuwyic.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/grmuroaro.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/golwsbrrf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gotauwlti.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gczvtdufq.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gxjadcuge.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gxzakmcsk.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gtksawocs.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gjpjweoab.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gvyquxoyk.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/ghkmpdbdw.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gmrqjulgw.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gcuoeofvh.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gxonogobz.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gsicizaut.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gevxdznan.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gxvqaonzp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/ginrcnrms.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gfmoaeoai.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gkyjrvmuv.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gprcwynnb.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gvsnwxyvd.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/guuqekisa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gvlxmzere.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/grahnhzpa.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gyamjcake.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gbxzoktis.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gkusduhnz.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gpkmbpdwz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gdgghneje.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gtphglwdx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gmwhzkpwq.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gkxlvxwqb.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gnulxxrdo.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gjntszutv.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gybrmatym.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/grhyownbz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gkkvlrcmd.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gkavwoxza.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gebsyznnn.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gddxozqir.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gippfopxo.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gfzmckmif.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gsyhmtulu.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gncuwzbjg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gwpgbuflw.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gtgwlzgea.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gcitncugk.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/ggzrylomr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gzawnjhjp.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gvirowgne.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gsywxcobr.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gbhpmojkg.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gxvtwzjzg.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gfiaaodkn.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gxefaatat.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gvquhccfe.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gtpaayaja.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gavyoxwob.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/grefjbbey.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/glsojkeis.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gmeoqkicz.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/guqwpqbqc.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gstlguumn.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gjawbsewe.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gkftolzns.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gjeeebvmg.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/ghlozxuvc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gyimoyydo.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gxefbxewz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gkuvfadae.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gdaztdvlx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gdooituab.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gzqkhwuvy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gasujrwjt.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gkruxacac.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gubgmmlzz.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gjouchexw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gstyjwfga.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/goeoaqwik.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ghfdeaeyb.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gnymmabkz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gjuqzmkcm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gkgibighf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gvceowkke.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gbrwnjuuc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/guqbcrlmq.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gkjynkkpt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/glgcievmf.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/ggcwbduyt.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gqrylqtol.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gsvvgpijz.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gikdwqdzq.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gutzgfznb.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gpronsczn.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gcneqbshh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gjfkedibp.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gyykufogh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gcfwoaule.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gnonfvmxq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/ggiwkaxvq.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gtuirawdr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gmktmrqjz.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gywfvtxmc.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gaokhhdsa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gvypgwytj.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gyszsvjry.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gpimhsxcj.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gmafksozk.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/glaezyfth.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gdtghadai.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gvaqytscn.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gfjzipfuk.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gjptqdnpu.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gyotpsglt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gtiapysqp.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gdyafighl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gizttxbmj.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/ggjffyzdm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gxraeedji.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/ghgwbhpxi.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gvpygyler.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/giyrbetvx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gbluviecn.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gsyxozwjl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gzsfuwbqp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gezxtcwcy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gygvdrpnw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grzppndjp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gndgddkwk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfwmugher.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gowlpvfhy.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gtjqaxrni.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gqysdrecf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gkrlwvjwa.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gpqgjtlxl.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gskcinusu.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gketuaclm.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gelhgzqle.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gfbuuiiqr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gymogzzqq.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gdhialxfl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gprggxtsp.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gczmbdeoq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gstkhptkx.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gxpovqkns.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/giwzyvohn.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gfhlindxt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gpgtuctwm.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gvmytdxme.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/ghvvektta.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gwjvuzzkf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gynqwwapr.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gymbfedyl.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gauvfvbht.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gtnukglsz.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gkjncjqqx.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gyefnxvmi.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/glsxmfwpd.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gceooykgv.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gnhzfjhaf.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gadqjkwkq.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gqdagmzll.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gjjymacqd.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gnfxmzjvf.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gmdvgsfja.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gyiaytdpy.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gjuxkmbig.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gzhamjdac.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gncmbrevn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gqcqbexeh.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/goglmveis.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gcyghcame.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gbqobrrae.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gklnlpbsz.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gkqkoylqa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gikfsolcp.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gjvubcqon.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/grswopdxg.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gvsahrqmq.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gredhluip.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gexfjmcys.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gflottjjk.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/ggdbiyywi.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gqouyzkug.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/ggnqbjdav.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gzwgrzyso.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gidqlbsyv.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/guwkehvfh.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gzhewtumj.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gyuapwnwp.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gugmgaqis.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gbxvekcyo.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gzunmsuuc.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gqjarkepo.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/geaxnmvqv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gniscidas.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gnhxcccqq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gbmllhcsy.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/ggbnwsxeb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gtefghvsn.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gfpgwhvhq.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gthowdsdo.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gpabvitax.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/glddxvwlt.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/grqegyuvp.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gnemjpgci.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/ghzvwmdhm.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gksmahvnn.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/goptaxbuu.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gyurlxych.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcqiwxuaz.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gdnksaews.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gsyexyzbq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gbxhcehgf.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gegxplpzc.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/grczvgdvn.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/goqepmfps.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gzdozucps.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gwtlgnpxc.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gcapyngfb.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/ggyrtfwyz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gdxqpqhvw.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gozqfhdqj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gvukctgqa.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gfbrcrbxs.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gbfoivurx.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gipyojieo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gmyxweqil.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gvsyqbtqa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gwgserfee.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gyywfeotz.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/guibrpsva.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gvhjisbzb.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gtravsoad.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gunlgkbbg.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gqhjbczvk.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gzgzbuxxa.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gbqcjcwod.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gucppkjqk.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gfzealjga.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gqwziekff.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gkpcmsthb.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/ghysauffs.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gqqobawmp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gjdmwzfxq.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gzidrjrep.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gjgytsjpn.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gkkcqjmxt.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/glhbslxfg.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gokjgccpd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/ggxhdhblc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glcowrkdh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gpurpuyzx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzdnpjnvl.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gtjkewqyk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gmvcexocu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gmxlhpiof.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gpsrzggnz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gtneuqvam.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gotdwoczl.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gkaimhglk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gscygspiq.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gnkkgpbeb.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gepjdpscb.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gwhwxyfdu.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gtdgbddoe.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/girowyoee.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gzgcaejdx.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gwvlqurra.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/greomnabq.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gedoczgvb.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gicqefsdf.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gouqsqswn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gawljdidm.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gcjfasztx.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpfmwsopj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gsafprwos.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/grpaewajm.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gtkucnbbk.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/guuytinyr.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gbteaanck.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gfjsmdzph.sHtML


<!-- 参考信息 -->