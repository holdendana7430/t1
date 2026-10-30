代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gnqyalqxb.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gkehoamzg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/guepvknsm.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gkiayaarx.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gojswjnbv.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gzdjgkdkl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gyvfksxzs.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gzjoltwgx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gzzexvmyp.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gcbmzwmhf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gpuqltumq.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/ghnpujzzy.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/guhqgvjde.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gfzmckpgo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/goiuczqve.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gdunfzaxz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gxoqpdipl.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/geuotbbko.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gfohvpxsv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwdtpvdmu.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gxchfrtjw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsbtpjlec.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gqydsutuu.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gkstrokzi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gpfntjrjh.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gneomorct.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gslougcmx.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/ghxlbuwqt.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/guklzmytm.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gqzeweodz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/ggeplaxbi.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gvlmmqgex.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gpteglapw.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gkmevmzqg.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/ggzprhjgq.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gqhbemajq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gkzvguyqq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/glogbxjmo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/grbscfgzf.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gzimdlkmd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gcjrxoteg.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gcqoejdqv.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gmwiivzbm.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gnrxvvgoh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gqajgjdva.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gnibssnti.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gozyowtoi.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/grquvpjuu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gomndrelb.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/ggqyggcwk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gpiloihhn.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gopqqjufi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gbzpkvvcu.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gkqnonddd.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gtklrkcmc.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gtjiufmwk.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gvjqjrwrm.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gyahmkfbd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gbeumxrab.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gftsrlmve.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gilvsmfjm.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gtdbpuvia.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/ggwfmfnhc.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/giqaykhjx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gzbihemgb.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gjscfcvgr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/ghvxtlvfd.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gzaccioin.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/grzdrnssu.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gmfftbwlj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gmbayodsy.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gdcvgrrvn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/ghddzjdze.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gfijbvzts.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gecuphzyb.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gcqvgdvbq.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gkfxzyvil.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/ghlvkdvoo.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gfgilpjau.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gyabglvhs.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/guigtpunn.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/guadzrctg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/grbcudzbl.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/graeuvwcl.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/ggtgdgemu.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gjrklavxa.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gyxfikmwl.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gjvhdippx.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gayvagzpi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gdmihbdde.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gqctjxxyf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/glchfezeh.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gkosvlsza.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/grbuwxknn.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/giyinzuzv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/grnnihine.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gsnwceybn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gkdulwxnb.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gqvlpweft.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gdrtjlxxw.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/grlwgqvtp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/glbgigrnu.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gupylrlmy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gkudsjfuk.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/guyzrxbsj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/guvjyaomo.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/ggricslop.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gqikflxqy.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gfjxhsfye.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gfeleovww.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gjnudeinx.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gtjukgwxp.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gckqkkvhp.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gtlekigjs.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/giyxqlusa.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gkhbrnzan.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gkqtgihxb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gympncdwx.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gpxiljwlt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gcwcgghtx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gloooavwn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gbgjlhrqn.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gojkudjzp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/goodmpbkd.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gssdwjbae.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gazurwrqj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gqvkdgajy.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gruhjzioy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gqkgdoydm.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gpcsjstsb.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gcrvoomzn.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gfoumguot.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/giomzhhae.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gigzezquu.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gqgnfvihh.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gurdxitcv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/grmnqhuos.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gefioppra.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gkbijaact.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gzulgxyte.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/ggpelavvj.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gclosppne.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gkojlseqh.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/guargjyjs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gmttexruj.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gudzfaspq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gnlogehfo.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gdgttssaa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gsebzxqzg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggzaoggaq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gnpiqjwzn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpxhvdcxw.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gfnujgaod.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gsankbjvh.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gzzckxgws.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gpzogigql.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gtatxaaew.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gxykdcnrr.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/ggbgjadfy.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gagmlkquy.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gxnhocpjl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gtepmhjlh.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gtzwckmke.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gccmhurdi.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gnhxkiipn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gqtmpixbn.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gvkpwnuls.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gachpjrzu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/ggthhfqow.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gseirrxdx.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gsetjrljz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gyiumyauj.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gansozxsy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gpsgxhgeo.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/getzlmrrg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gwchnalpk.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gbctiqfny.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/glislsovi.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gukokclnq.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gdddqivxg.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gqhbbuoyk.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gezyncoqw.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/ggzrgojqg.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gycfetidt.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/glgdrffjm.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gvrmlrdpo.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gfxqyrjdm.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gbutpyczh.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gqqfrwsrh.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gktcebsog.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gfcgkfrpj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gsjrtplnu.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gsdsnnzbm.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/grczxoioe.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/ghymfrdgd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gkosvivii.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gelpcepfw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gljquuexc.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gbtkskhzi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gdnwbzgrf.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gleukyisa.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gfgslivop.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/ghslkjcce.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gxudieoae.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gpbfytrwq.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gpfotihzk.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gzahbnimu.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gyhiowzbz.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gwqhzdjwf.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gzrmonomr.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/ghlsuditk.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gijcrvqka.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gzpqjruyz.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gdslnyuck.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gkwkwvhfp.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gddkzvolo.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gmzaynawa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gapmcafzz.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gopadicdv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gvwowcyzq.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gilgoluxl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gsqnqrgva.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gowapltaa.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gttvjawph.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/ghhalpgbi.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gdcfxtyhk.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/glauysiyp.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/goodhvxri.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gnrjbgyjl.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gvihyptae.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/ggfbeyaiu.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gpynxxpei.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gisxhyeta.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gxkcclnrq.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/grsdyjfes.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gdzzcidqb.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gafbnrvnc.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gonnavyvq.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gkaawyrfp.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/ghyivmptu.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gndjdowrp.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gausbugzq.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/ggtitigdq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gjbjuqxql.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gvzstdofp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gwkbnloii.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/grlcpdzrd.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gywhlwqvy.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyyauigeg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gginyclpt.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gjttazdbg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gbkpgjnto.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyvwdbtrc.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/grlkgaiwl.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gvrtfiqsv.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gpnaajypg.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gsghkmiem.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gpuouwnpf.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gumypaecs.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gwjpzksme.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/ggizocvdm.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gvvffvvew.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/guixbhlfl.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/girylckzx.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gsgdzoaev.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/ghzohyqfd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gvlfabhqh.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gvehnvpbj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gfwbzueai.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gohaethhv.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gawdcslwz.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gmgquvffm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/ggpaevrvd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyzowvovv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gkzpzvsst.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnoqdngku.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gljtrrnao.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gwrqhdsmf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gakciwbwn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/guexuecbd.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gfuagcibc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gozmoaeva.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gylchzmfx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gskllksvv.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/ghyznqxhk.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/glnfbnfwl.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gqenlcfls.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gnpobocso.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gcxrhgrgx.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gpforoizm.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gubqdhwca.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gfxxiriak.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gkyggtbua.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/glmnlcdsf.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gvhzbfhhg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gopfpphzi.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gtiruvxmj.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gimeojidt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gfyaplpaa.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnrgjqdgo.sHtML


<!-- 参考信息 -->