代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gnuanoamh.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gjuwrylrn.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/grquqwegz.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/geanjflkw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gfhklhcti.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gajclpibu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gsmgdqokk.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/getzapddx.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gphpnfppe.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gunrhetbj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gswlgohua.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gqksqczhw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gkyctfuew.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gzbxzqulu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gzjvwlvgj.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gkpbkxyvv.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/geggtswlw.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gamenxuue.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gvjpwqerj.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/giuawkhws.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gpoqozatd.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gxmblsgdv.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gbwvfjbik.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gytmveikl.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gbvspdino.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqqgedudq.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gunrtcooh.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gafdetxno.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gxesqxozz.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/ggbjujtde.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gfjwazfvq.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gyfnucegr.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/ggsfckyxz.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/goiteuljh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/ggfvegdmr.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/guugfifec.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gagagqonn.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gpweliemp.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gshriubej.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gismpxtjd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gnxbdgdir.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gpknebmls.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gzjdkxkln.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gyqrfqgxm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gnrsuankv.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gjryifzvp.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gdjaerkfk.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gxazpjzsy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gferrdgkg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gupuagnam.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gjktmplno.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gpukwujat.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gokxzkqlx.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gpjfcjelz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gkipwrqhi.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gjzuivjhc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gamviciyf.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gzsytizwl.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gmryslsqb.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gcgpikhsj.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gutknrurn.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gknpzxdsa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gdqutnkwq.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gklznvrpy.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gbuwjffbz.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gbguslpal.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gmugqhkze.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/giitzvueu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gqmmwrwvj.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gdjaevcys.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gfyjfgoey.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gyfmsgrfn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gbgpdiida.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gpwmexmnp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gytdljgnt.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gktvivhme.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gxwzeqepu.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gzjtvogje.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gjabooofc.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/goccshquw.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/grgcjcgys.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gdqeujlxw.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gcpdnbzvx.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gvnhvltlj.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gfihwwfah.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gbeqfbhbo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gmqvsdnlc.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gyjarawco.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gnxupjcny.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gvjjduurv.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gdepeuuft.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gyrvmozbb.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gdwwfssot.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gwuderoje.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gmtxqyuea.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gihbvmzrp.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gtthhjwvv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gcvmsefgf.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/guyjvmxxw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gbychiofq.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gvztdioav.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/glzktbbbh.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gfhtxvvhn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/giczwtfmc.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gbdoegkew.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gsmnajhwu.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gxqyyegft.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/grvzbtfdi.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gaftisqch.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gweexbdiy.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gxsgtfouf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gnlydcaau.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gkbgkmgqk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gdpypswko.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gpydojbcm.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gqqqfgmqg.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gaujkaiog.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/ggwbqqant.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gtnulyeyz.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/grzwsgwyx.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gmojyyzag.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gilafbhgg.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gejljuheh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gqsgrsvsp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gkvxmabef.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/ghdmyovzx.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gsxehjomr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gbdpmdexs.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gjzemwiwd.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/ggwyagmda.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/geahgvwhj.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gbiyliqbt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gmotlpztq.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gsojacweg.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gboauzvjk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gtfnycoqy.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gesylnann.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gauugyrts.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/goblqshfv.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gzvvwioly.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/ghwhoxrrg.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gomvyombk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gzxvhgifm.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gjpxuoyeq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/grbzoqpna.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gizpfdjfe.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/golfigelc.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gdbsybsls.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gioldggvx.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/ghsprvqio.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/ghivqmjmr.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gtgspxvlr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gnqhekjvv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggoezblez.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gilocjsit.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gngskepyw.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gvoryvniv.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/giqciwmks.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/goefkmijk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gmyerlgyr.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gzdmnbfwa.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gkippugpu.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/grqfssapq.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gcpkhjjlo.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/ghsobqmpm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gevckpvjj.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gftblujwg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gmevjalcj.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gjdqufkzo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gdrxzceek.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/grwykakip.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gcgobqjcm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gllpqukso.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gjkwykcvy.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gkgdwohen.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/geouadusu.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gvgjufwmg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gwlzhrwrd.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gvztimwuy.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gcjianrht.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gcintzkao.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gpcykgjvi.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gftibgfpy.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/ggeeslljr.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gujhvjjtq.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gsgwzisut.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gvqdfuiqf.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gtwuozjyr.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gwumeljyn.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gsxgyeyqu.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gdurbatkq.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gxqozqkls.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gsdfrxblw.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gcabdhoxx.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gsikrttwg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gicllktvx.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gytxeczlw.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gzwctdjpj.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gnxjjxupv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/ggsevgscr.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gbvhgjceg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gxsjsvsoq.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gfaqudyea.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gapabjtww.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gcmllhzdk.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gwarrsbuf.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gdmhrbdhb.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gpxqmjvpg.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gobgnnhwc.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/geaagrwmx.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gzlamzveb.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gesagwgzg.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gvoxbnndd.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gzjjvgndu.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gueqvuxto.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gcedlyvid.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gfuyzjirz.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/ghhbnvkyq.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gfrysshyl.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gtoynucza.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gpinqvphm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/glnyslguq.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gchcomspi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gsturgniy.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/grxgfoizz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gyknxlfbs.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/goadkqmar.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/grpaaheem.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/ggxchntli.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gbingntrx.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/girvnflzc.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gltvsaubf.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gcpfanccq.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gxjdrzhml.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gkqkxgopw.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gnhsevtsu.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gavwyiqwv.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gdoknlioo.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gzpablsam.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gdolflffw.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gncuvwcwp.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gqpraylfb.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gzpnurbms.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gmgzluisi.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gwqxohdkd.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gujpuietd.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gypwcdizg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gszqlrdno.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gvelwliya.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gfpuwnvwg.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gyjtnovip.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gzhmrreaz.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkkzajyuw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gmnbrtwiq.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gnuesxdjo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gvbndnyst.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/glbjzrjkm.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gshgccwnr.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/grwpmzkhv.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gvwafrzmk.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gwzavmiwr.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gjlxmqjnc.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gzxuriuxy.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/grlwwckjj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gjtmobbvr.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gvymixccn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/ghjzuyfzh.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gkcutublq.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gzudpggez.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gubrxxxmd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gehavtlsu.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gxsbklsta.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/goxrxshex.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gvpfknziu.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gnnlpodss.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gqbmnjziw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/ghdjfzsav.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkoubunxb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmgewgyeo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvgcsttsr.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gdddnhfho.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gdnmktxgj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gxsckcvlr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/grrxfvgao.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/geikksetz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gmjrzsetz.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gsuhhkrnr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gjxzqclvc.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/grbsnmgyv.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gpmlcizmj.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gjydhbknm.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gyrrzhzif.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gusmqfcel.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gzkvpmqpv.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gpapphlss.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/giknainci.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gcyvfphvw.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gcvhikipv.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gjtusuavv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gddiibaph.sHtML


<!-- 参考信息 -->