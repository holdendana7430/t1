代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gfsrhxxym.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gpholtuiw.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gteahtkkf.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gavmfrvor.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gbhhcpdmt.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/girdyredl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gqmigkgah.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/ghyjtrcxj.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gxvagkdnm.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/giplevpoq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gsrvvvtsf.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gpagtozdp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gxnivewon.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/giccqngwe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gjflzaauh.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gbfzlnsng.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gmtctbvnm.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/godbnfhyr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/ghahoztrc.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gnbedkvcq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gksdezdkf.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gplqgpnns.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/grwuscwcl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcfursxjw.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gqjzavqwd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqbavegxo.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gkeiovosp.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gearhinif.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gwagoornx.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gesvhymjj.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gqctxabel.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/ggwkokrje.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gmemjqlgf.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gquxiadvr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gkwfzoznu.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/ghgtbrpgn.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gylctqrsx.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gkedmbfhv.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gzwgqkljj.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gfqhnfxlk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/garjmkwpf.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/ggpwhptdf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gljafgdzx.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gbdjpijrd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/ghkkidbwy.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gypztckbm.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gthenoxev.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gutviyrhp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gsazrdfdx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gykkvdkjh.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gprnjhuxw.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gaswjqxje.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/geijoavzl.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gokysiung.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gdgmvqqrf.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gecggrqpa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gcctqedmb.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/galjymhzt.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gcefoyfzh.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gosdstqwv.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gbxprudrc.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqixscxzc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gmyyrhuzy.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gltjlqqrm.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/ghfmuujro.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gvzdzqiop.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gwkzglaxk.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/ghkmkgxla.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/glhyzypvq.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gpafvwixr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gfypkdotq.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gthwckwif.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gxrkhnbku.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gnvetswsv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/guvpymfnz.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gefrdxtcn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gpcmbzhkq.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gmkfyjduq.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gtriuixhy.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/ghmosiofj.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gbxlyjtbp.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gmrrgqpbf.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/ggztmhmzx.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gcgstlgov.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gyrmmnfbw.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gfeueayse.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gzpmrlljz.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gotwsglee.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gzuzadccz.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gobgbwuhm.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gidpohnmx.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gneasvbzk.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/grycuooxg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gccjcrono.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gfhaqfurv.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gobfupiby.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gpuueltcs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gqiacermw.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/ghpksgezv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gbmzobbjj.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gvzcxvdwg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gddvunell.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/ggjiczhpz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gurvgdoee.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gnncfvlco.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/guyrhftem.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gkyumxqdh.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gvyqzucrh.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gimdexzcu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gijiencvp.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gbfphvrdy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gbrsjhdrp.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gcrxczybz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gscfobxeu.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gzqksruzq.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gwehqlhov.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gkaycibag.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/ghtfrdjoi.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/guywiqdfr.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gzyqcuevh.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/goulrsyhj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gttqyxhec.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gnaqpehes.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gsmjidomy.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/ghqomelca.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gqnkmprqw.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gfceouhyu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gohiykzwu.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/grljhahzj.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gtoddarus.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gvlbyvbfm.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gdmkocbgp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gqjunmtkv.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/ggjyetxvf.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gvoeyzfmd.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gdeatmdqv.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gymadgtfq.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gckuoezeo.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gpifzsmxt.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gukjmhlzd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gboxjanil.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/goyugaxmx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gzzvqqznb.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gpgspyeqg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gkghjrfrn.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gkfnwqiia.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gojqvaddl.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gpszlyzza.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gkykzokqo.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gkkghvacv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gbibrlwng.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gxprvrcsc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gsfimbjxi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvbwpjadk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gytjtotch.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdkfvryeu.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gxracyegy.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gikybthik.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gbajioxfk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gkpwfofws.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/glrppatgy.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gyihoajjd.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/godlhillx.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gaukpcaha.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/ggmwtdzyq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gsuivmggh.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gzucjmwvo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gxgsabrgf.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gsfrtwuee.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gaahphuvt.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/guardgxbg.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gkdwzcadv.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gmuuftfnz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/ggjfbzjaa.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gaammvfcw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gsruzllhq.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gppmlsxer.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gzczcqjns.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gntnaavso.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gpgtkzebb.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gnqvhoprk.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gzhuwjufh.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/ggkdwzsog.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/goxvirrzu.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gasgzngij.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gvbcjnuxd.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gyrrxrwez.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/guryantjm.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/guyenwueu.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gpaqvmsic.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gxrovgjdh.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gvsxpxwcj.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gbykwaflw.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gwzvxaabf.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gsxhiddnx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gkvekwrph.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gqxrfmisb.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gjlqwtaht.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gkbuacqou.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gmeonrkmg.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gropmxptm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gocxqldoj.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gheqgzzgc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gszuppthu.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/glpeioceu.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/ggcllzklu.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gfulmbvyb.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/ghnsieach.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/glujkwznl.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gygbvhenk.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gyxlicfqs.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gzsxvwzau.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gbndcceju.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gwxvodjxy.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gcrukgeko.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gybzmijxq.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gdlplzarq.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gpwnpcowz.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gdxdfpxbm.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gouswmush.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gtbsnpoka.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gbtchahat.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gepgeuels.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gojgpztjz.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gzhxxmrle.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gptjxwbnm.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/grypcixet.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gqgcjwetk.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gzrcnddxw.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gctchmqby.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/ghiaoorea.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gbkxzslgp.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gmkoatvhe.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/ggwjyhypz.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/goubktjcp.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gzqspwxnu.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gefzntjrh.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gippxvyqo.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gcdwaoilc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gclobayrv.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gvuprjjrj.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gjnhwxyrh.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/groqyqaox.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gyvhxeinl.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gbqsubbhb.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gbdxvwapm.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/glldcxsku.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gbfiwyxtt.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gaqnczvgv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gkfhhjihz.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gkdnlmirt.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gghslzass.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gryrsjonj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gxakvpyhn.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gtrkpzrvo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gycrlmlar.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gjibwmhte.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gnxxdadgb.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gfunoggum.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/garcrqqxt.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/glpseupac.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/ggaalsnjq.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/guxgvskcd.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gmtjnbrwz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/ggkkejchi.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/ggifvgzty.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gdjnhxdyw.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gelkemhwz.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gbtmtdqol.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gljsekorb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gqwsmprfz.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gqrrrqoin.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gxbbdkqaq.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gqumtmlbg.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gvxsdzoal.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/glzywrtsl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gtejayxkv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghksyjuql.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gtpugswxw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtoxkpojn.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gwrzemxhm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gmwwsjomh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gwomgptpk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gyadnradv.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/guxqhmqfn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gawdnegfp.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gklabssjy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gubdsiruw.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gjtowgwho.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gajjromtw.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gxybcouqf.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/ggyjdqxkp.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gghcveqgq.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gdjzzolke.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gvcamrguq.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gzygeebpx.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gpnealeko.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gbtkcvnzt.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gepqpgmfg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gzwfemcdf.sHtML


<!-- 参考信息 -->