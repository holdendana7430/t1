代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gimqftlub.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/ggytugsgu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/guousktko.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakuxgvwv.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gtlvljddi.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxmivjoo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfjvovira.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdylwhxpk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gswfyzvym.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwtunryd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gntbznlfo.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gooekmtwk.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gffhlarii.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gadjtjuwj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcujkzrfk.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjfzbcyr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzmweizya.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkxqnuul.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gccxtlqet.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glulmmvro.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuulizgi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmwhwyimr.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjnnwbfa.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gerpcuthp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxvawcnon.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/glnrringw.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gyxdumwbp.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gclgewgyc.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcnahlwy.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gecyolxaf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/guajwkoek.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgpztpci.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtrvvech.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gktmqahsw.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtfxoeit.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaorxubn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/ghetlzqjp.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/grixlbvgl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmbpfulb.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gnluwrptf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gthgsrlfq.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gcqosibau.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gjmmgdnfz.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grnkmzagy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gblramsur.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gqwzabyfm.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvykbuii.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gugmpdqeo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguhpjonq.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxmrgxex.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhygpovx.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/ggdjfcvin.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/geijuokfg.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaeygezu.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/ghkiaaczf.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/glsvyzsua.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gdhvdjsea.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gfhzjomtg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqasyrzt.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gdhkikoyq.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlcxqfzl.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/guvjdpgym.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmnqogbo.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/giohscfjj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpczgwogk.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/geycvqgjd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/graivqsfa.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnyhqiev.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcristdyt.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtejwqzv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzfayiic.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gyggkfnpb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gqojpvrbi.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/ggsueqluf.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvryrmwzi.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcthxhke.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaqkgomq.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gwatcmqzn.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gqbeqsbmb.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnukpnxvm.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gobqqzebb.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlbrcyle.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/grmudgtsu.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqswcftpr.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbksqvoub.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepshlnds.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/giazdhlup.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweevhkvf.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gyripxrvw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkmhdtnu.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/guewzrmsj.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gyrtofkct.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhihkyvh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gmwazvzxu.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gddanwcxr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpitrtse.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gryovqsjn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/glvoiwcnt.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gvuynxjqp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegpsrwvw.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gaddtjdds.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/govdjyujf.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwbzpnymm.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtqpiusv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunncdrcz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gyujfxvjl.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvwulnbi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqacvuyq.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gjhvykzes.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gakeqgher.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gtqvvfjwu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gabzqcxtg.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gjppfmbxh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gguwpjzdu.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gwhgnnlrd.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gycevzhlz.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclcgibjy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gqktpghuu.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gfepmuccv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpcafxvs.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiberogt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guftfndip.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrbpsjzq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggozhhkml.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gftajzopx.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjxytkmr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaxmqmsh.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gnfigrdwp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeocjzyr.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotywseic.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/ghimyfkut.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzshramx.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvkecyyk.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gagicwncs.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gojrdeqfw.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gggihrmjj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdjcckme.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaezwbkh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxhxslox.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/glaflfklp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvalijugd.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gwdphqkkz.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdspmlaxf.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gwvttxcub.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrznwfpd.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgnltjam.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujvpouon.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gompqzkfj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gvjaysfih.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkbdsmhf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdyxdcaq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdtcdmle.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gtadjruuh.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbydhotx.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gksjeqkrw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gqtgquokf.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwfotvfs.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gnvrgysin.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gozgprhjw.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewluzcfk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godconqzl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwhfysnh.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gewqyotwb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwqxvoeu.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gopjvjgeq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gjuecawov.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqbxzhjb.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gauyhuxvy.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gazphnikf.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeocqiba.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzptkpvg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gestfpcps.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gugnbiycj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gcbxzykrn.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gugewbuug.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxtwtbzl.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gauuvzyar.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihbmgmfy.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gcgedhojv.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/grkpohiui.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gdkvzmfub.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlxfybzu.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gniwyigwn.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvddsufhb.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gdviyhdgo.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyaecyyz.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gbbbxalrh.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrtnywzz.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrjmplua.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmuuffal.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gxlhqwufy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gnorutiik.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbefttmz.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokwcixqt.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoxksugk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gfjfsbpfh.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwowennn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfmbzrwq.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gucfkjwux.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwwkwnrp.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgytibuh.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gafqkmqys.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlwkosbk.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkzbfngw.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhbqlirq.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gnrqwrwcz.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gujyjaxov.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpglwqjbj.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/grdaewpfy.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfokfrsw.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gyobkkuxb.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gorstujgk.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/garjsqczs.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmxcqlqj.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiwrpiyb.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/ggrnvpogt.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gagkariax.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gttkxlkgz.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/geqapggqe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/goigybstv.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfhehjkw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaiwslmm.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnvheasao.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gcndqlwec.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwmdfxcl.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvishizpd.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/glnmzhflh.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gpcsalksy.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gcgpjlrno.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixyohygu.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gjexrzlkw.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/glogxqcpx.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxqkerfk.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gqupxjnjt.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnsqgpva.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gakcykanw.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/ghuhuagao.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/giuuxrila.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gieeohggq.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbrhtctix.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqazdcvz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfwefmww.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/govyygmrl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbmyibrgs.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gkjrgyiex.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gambkciqz.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggetatgvh.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfozmmji.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsewhknoh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glemagxpd.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsyuvmai.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfirkdrs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdgibcbw.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvdfeqba.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gweotxzlj.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjahgbpsc.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gpnyjkypd.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gebvsdbvd.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gegzeluwa.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gtymcvwyk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkxwrqwv.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gpsnajuyu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gspaqfmdf.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gngdjveap.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/glanizndi.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gonlqsdgi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gbxyscamd.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzotpaxo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gcxxqrcul.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gtsqelchf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugeehevp.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/grjwakeur.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/ggvmqqfpu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtszistee.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/grwrippmv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gggtzortv.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gjlzgkmrq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfhffcia.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqrcvgev.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gesdpavwa.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasgdiqas.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddrqnxrl.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqcmnhpv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gdodtnhbs.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gupzuhvsg.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gunsflyzj.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gbplomlcs.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwdgeozt.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/giwzofylr.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvphinee.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gmrzegenn.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gjxusetdj.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeavnrqf.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpuelzvl.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gjsnwctbn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsmiokbq.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafkmouri.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbhejvml.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobbvymqj.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gworjhwkg.sHtML


<!-- 参考信息 -->