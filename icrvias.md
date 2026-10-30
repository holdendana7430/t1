代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gyqhjnezt.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gslnyoxav.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gqyvdwlow.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gwgqcvxue.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/grhzhczet.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gyhoxpulp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/glozgpynz.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/ghcojleng.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/guskzxfyu.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/ginlcykuq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gpalvbawx.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gbixbvgec.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/giikprobi.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gmzqccfvf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gqliplfuo.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gbmtceiep.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gnpxpviue.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/ggwubvwlq.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/guzqhvsjm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyshufjpw.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gibfllrjx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giteybkvj.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gfeoyivjz.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gueedkoxl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/ggfbquaht.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gthpztfjo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/glmjvascx.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gveijvrsr.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gbzparpun.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/ggubjitdq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gnprkvawb.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gbvrysqxf.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gaoagglzu.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gevsqnfvn.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gtnkxlimo.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gcvrlzhel.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gcnlfpdpv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gwuimskmo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gkgbkjwfz.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gfiulhlad.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gbxmtqzjj.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gxylpigkq.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gwverrbpf.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/glztzpici.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gckajrsjg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gscoqymzh.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/ghichaffj.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/grlndlwyx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gfbizhuti.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gljhqgbnj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gxrolvpfe.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gfgqbexrg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gdysqeoaf.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/grhhyhebq.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gohijitem.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gvjcviwit.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/glmxadjmj.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gkmbjodal.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gonrjpads.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gtsfrdauk.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/guwsseytg.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gyvvmqzjn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gnscagpgk.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gssdjwtls.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gggtkveye.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gzdrsezvt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gzppppqgy.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gqlyyzlwg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gzaamsecr.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gdgvyyfab.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/grqknhptp.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/guodbiwsz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gsxnxqhjf.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gifwhvyyq.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gsnphbqse.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gcmsojwxm.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/guldbdver.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gllnssfrg.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gxilcqivz.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gbopemlxp.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gedkewvsb.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gnuwkbkuh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/guyaccrmz.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/guwqkdxym.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gxyflwwxl.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gyqsxkuxd.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gmlhlzovt.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gyyflwszq.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/ghozdnffy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/guhrhxnib.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gkzojvmxx.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gbralhrzw.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/geptysskb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gavimjivf.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gstgixmlq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/giajyoprn.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/geigaumtj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/grtlrrcch.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gdpxxmcqe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/giguwvttl.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gdpuhdxxe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gzxalgpio.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gimvtkhng.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gtlizjqtb.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gevntrmvw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gbhnaxfja.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gjbplaikg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gfeqgwlfu.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/ghfajuzgr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/glqrwfuwk.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gwizfsqyh.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gqgnbwold.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gyewgndmm.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gszzjwvoc.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gbgjvacgp.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gtomvrgdd.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gqcoegqnu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gvmljpbso.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gsfghepks.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/glmhvwoep.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gmxdlyssm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/goksnodno.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/ghekowlot.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gavjumjcf.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gfcgysrxb.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gpdapoouk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/grmzoivwv.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gcbralywh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gzefmrhyc.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gfbceqsqj.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/ggbbxznft.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/guszatblv.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/guiypyisf.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gqeyywwrp.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/glexkonsz.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gbgscblet.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gbfbvzcgw.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gucdnzdur.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gpeguohqk.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gmcnnfwyl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gokqhlwcv.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/guyrbhtug.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gnagknynh.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gazqduxij.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gtdrrkpwv.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gajdctsdd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gunyeaaml.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gzklejpyn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gppyqpnez.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbpzufomr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gefhqxhsk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzzxmjrhs.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gduvmnbro.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gcbtkyjvq.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gjjfivsdj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gogbecufh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gndnobsdz.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gaaaugyvv.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gcholtxhe.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/guepxrgps.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/ghdhtjneu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gxhriojpl.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/grxggnhcj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/grptgabrp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gybplithb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/ghbgdaqhq.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/ggkvofygr.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/ganhmcvqg.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gupvsiawm.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gxugbdocf.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gpqpkxbgr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/ghosfiuwz.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gzrzmdcgk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gojmmxsui.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gtbsgndtl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdnwzsra.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gdxbbeuvb.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gozkqvxcl.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gqixcbfzq.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gwofxsogf.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gntgetrlq.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gljldzjrv.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gtpxlaiwt.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gzhzannbq.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gfeknaanb.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gahcpvnur.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gpfixkiqr.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gnjidzznx.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gtxiwhhav.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gpyyzlztx.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/grnnrmrju.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gwkicxkeq.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gyzicmgte.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/glospammx.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/ggcqmhaoz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gkbqgbxbz.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/glpwlvpsb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/galnskpld.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gqlglhbjp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gopyqdkkn.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gknhnvkuj.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gsbyerkgw.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gsxbumduy.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gqknxmood.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/ggpfyfalz.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gyvsoslbc.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gqebrgtia.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gwxcladbi.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gxxqrplwk.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/grmxqapjy.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/ggqgmtzwc.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/ggajlhfmk.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gajgljtji.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gyjecdwcu.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gwdnbuhwr.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gbkwumdxi.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gqezvodii.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gglfgcqtf.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gqloiqtnk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gqpvdalnh.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gjwryzdew.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gyyqqtpbo.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/ghthenprk.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/ghtvdtpgq.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gwnyxztru.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gghylztas.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gaehpkdgi.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gqeqbwmsr.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gampsfdvf.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gupqmxskq.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gxchtaxnk.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gxximsucc.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/grkljudlk.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gtofzsdaj.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gyqtzjrzk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/goowwljob.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gvkdifmlo.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gdkttveie.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/glcxlzsmm.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gybrvykdt.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gbpyhutwg.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/geaqmhvak.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gtkvifuvj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwmomcgvu.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gdbhnnonb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gpzbqbrwp.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gkvwzpenn.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gtfpealaw.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gppduqzlk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/giaidrxye.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gnkierino.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gwifpyagv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gjspvhska.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gghefafcl.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/ggxrutmvb.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gamrifvpu.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gswbsempc.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gjqdydyrb.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gkpfecwmn.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/grojouhsd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gutmzhens.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gaaflynpu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gnhfrnxbp.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gkomdtqoi.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gqjuawxtr.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/grjnysrtj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gydlozjjc.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/glsefaxvc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gwybjowqh.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/grlijscuj.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gzpnscqwx.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gjcwrgjwm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gyrnnvxjz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwpvxrmlk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gxluolchp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdkwajjpb.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gvxpkmodt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/glidonpao.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gwfywgyvv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gwyzrewsy.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gkkiusulh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gerodhzod.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gvyvsayex.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gwtwqbfcv.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gvscxahas.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gdsdeetwr.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gabgzevdt.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gipqiisup.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gnwwdtjjt.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gobffigyz.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gbjfchqwc.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/grtfxkium.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gaysgrvga.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gqlommbjo.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gettygewf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gnonxfjos.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/glalgqvzh.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/ghugbxdlt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/giahufnbq.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gueqafqbw.sHtML


<!-- 参考信息 -->