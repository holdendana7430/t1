代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gqyfdqvow.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gkkmitduu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpwrfpbt.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqpxfpfl.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gwulrpfkz.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gqcmjmiaj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpsacqqb.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcqwbjrn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gjrgnxxdo.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfktekqec.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gsdklqgxs.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gokugrzla.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefzxwxii.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/guufrhgce.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gfyjckgey.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gmdivptzt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbytzcknq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gakxbulck.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezftzbjc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gaghpxaop.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gcclofgkk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdpnqtwd.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvlxsarq.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/glvayyfoh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhbahtqp.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goemkbegc.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gnlqchwzz.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfohhvdvn.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/grywxdpyn.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gurlkberj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/guizlfjpz.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoljmkqt.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gkruukbak.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjurzqfx.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gneujtpkc.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gwmfiexwt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gnbdlmgug.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhdvsymj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsitzravj.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvxeflcu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gztmjwcue.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gkckqrrvk.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnslslkzz.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiybtgwq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gsijiyubi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gtiajtowi.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gcogdjyvw.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzpjhloo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gdofiuasc.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gxvxbtqch.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gggcbmjtq.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gwxyttqgt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gqevqjedy.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdzwopvx.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbnltiok.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwgoagnm.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gmmnroaex.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/guppkrirg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmmyvqqk.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzcogddp.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gidrsysma.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gdujptvys.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhvyjfmn.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gznmtgmas.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbdkvmof.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gbttnkufx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/ggzjzuiwd.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttzmtysc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdniwwkf.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfenxoch.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/ginjzwzgq.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvwneehl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghosbycam.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gvtxznfvb.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gonmhhhez.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmwiyvtr.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbsipolo.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gafdxtzgm.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gyzfkivus.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtjeykeuq.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gbwicwbab.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdutznzfs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxrcihxc.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdongygv.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/grsexfdfz.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gofzpjekc.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gqmsoohdt.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gotlqtkwv.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgmqsljk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqapatnl.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gqbctociz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gbazqymbb.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gyamqhgqn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gohcnvvzs.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/grdhengsg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdfokmgml.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbzskqor.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gqlhjalnu.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjolmngkf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/golymhqwp.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gahytscej.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnwpixdk.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gobhafkwm.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gkcaxxljk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gphjpphyq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gbydfrhcr.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gndvndswk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/grszncbaf.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggfqhurhb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gmvhibokf.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/giiuthelo.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmizkeqky.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpobiyff.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjpwtiiz.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gimdozuwc.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gicseixaj.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gkiludide.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfllrgji.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gvjowjgha.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grcsiwtkl.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gmakxocso.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjxtnqldn.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/glrrbiocy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwctwodly.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/grcrffkgn.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdfcxhhtw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/grtsvyxyp.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gwqwoxrjo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjrksyef.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gcmxmjwaa.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gxczogtmz.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gbzjqusnc.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpyviwnc.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gnyfnkhya.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssmpcwuh.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gunyfjcpt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmauwwxx.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grydodsua.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/ggiqxqapq.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/ghpzpyqqu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpmdomvbv.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gtbfpsxuf.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrcbdsag.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccmzjfti.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuaccfid.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gihvzluun.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtsmkftj.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gahnamkow.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfwcorqp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgprpllx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjudlxdu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gypsfdoel.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gydvwdpjz.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gqopmozoa.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjrjuilkt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gwtemcogb.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gdzwksnvq.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxlmpivd.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gttzgqtri.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gopxvpqjq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdakqwglb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gdihhqxqj.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmfpchje.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoudsszq.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gznmgjpll.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvddvxfxv.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gvahbiasc.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/glctjbqms.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/geurywtcq.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gyoadzldt.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gozkvxsvy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gararqauj.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpsqagnn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gakyxbiee.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gocbqvsyy.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gzbbndcnw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpziegmp.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcogkstn.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/giukhqjnu.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggubtozoi.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gjikeavry.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwtviufn.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gslmrskgz.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxaunfqd.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxmxuzjf.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjuunled.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gefneszig.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gdnzrtqxc.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdajtbml.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/geklmexfj.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gobdinwnm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gbedgzgax.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gtljxvvny.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/guqbnuynh.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/ghagyclxc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqterkidl.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gendfrfqg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxnkbcku.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcuczxwy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtccmxus.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/guijnxwwz.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gwlhplvtm.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gurkrjjmu.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gyzphdcta.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gshmbfncg.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gzlqdrypb.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gqdekpdbi.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gudyikjos.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gwbmimsfb.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gnfaabluq.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gsofxsgtk.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gbbyzfbdl.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkgamxbo.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gskwkwylv.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkffgzacs.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxqbxipk.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwilercjp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gabdynfwv.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gpalosnyv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/ghkyzexxp.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosilzqhl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/giryibkns.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gouytqswr.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/grgebbbot.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsuxcaau.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtabmniq.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gdjlwqdaz.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gxxnojjzv.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcscisau.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gfkfppesa.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gvdlgtjoe.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrtceixn.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/goahfuguy.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gudmqozkm.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/ghvfacusi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/ghczxivbp.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfvlnzeb.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyezvazja.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gugeayddk.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giwfvzxlw.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gqgnveddl.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnitelswg.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/ghtzhdpyu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfipvynpb.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfghyusd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gapzcnoeq.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/grduyuoiu.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgtowhuu.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmywurkf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwquwedq.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbxtrhad.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmtwbubk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzjaahzw.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gsehbwclt.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ggsdlygik.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/groenuwfo.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjlcqcoi.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfciryxp.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwpdawnl.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyrfnkdk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhperqjh.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/givgcpgem.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gptctnkkx.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gyfsanecd.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvszbteac.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gqztbmmnn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gswdetfql.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmemwvbq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/goposerka.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gnlzjiguv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpboeluxt.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/guoiorgmn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghroksupn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grsffdhex.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gyatotmxa.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbskayimu.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gwurpjzcu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gmxkltfyv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gxwndwsyl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/greuajfrb.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gompubuel.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/glkufvhuk.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/groshiodl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggggunzzd.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gmlreslbj.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcshxdfrw.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gglbjixsp.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gdsrjvtrz.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gguddjkee.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gepavnrtu.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsyyawbm.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgzaqwsa.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflrwtgid.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtfjnyln.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gjapajprw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/guxiawhjo.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvvmuwjy.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gphczepay.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxcpbcah.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgcumnbb.sHtML


<!-- 参考信息 -->