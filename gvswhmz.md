代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/ghqkgmqnr.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gryhrcqqj.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gehicaeqi.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gibedbndh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gldaxhqdw.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gwxgogtqv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gdinqpuen.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gfaotfjcg.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gsxvjlqla.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gquzgfknc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gzdqydamm.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gtbogegvt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gnjcaqxzu.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/guqdtqzoe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gknusnzsx.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gqallckwi.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gsdfiaozw.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gcuremfyt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gcduniyfb.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gqkzwsaum.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gvncgjwej.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gjdjohbvv.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/ggflomqdd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdtwdlvhp.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gruwsexth.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grlyqbxmb.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gqrzcpstm.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gemfykidm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gdpnbfagc.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gtvtbquex.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gvgytzoji.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gszzwyxgq.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/glnredfqc.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/glzufghhu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gxipgrtyf.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gyajhtmxd.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gugfvfqjk.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/getlkuoge.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gdvggufza.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gcdqlyxfp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gpxgxwpyq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gdapjmmve.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gwofhsdfu.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/glpofbftd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gwonuunoq.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gpwlvblry.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gstuvvkvq.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gousmtepx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gxscwicrd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/ghdwitevh.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gnimuldtl.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/govxfrvbo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gqdepvtwp.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gmtaqdpwn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/geoasqjlt.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/geajyisio.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/ggqimtrlz.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/glragpmqu.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gqfmneewl.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gfhrvxjhe.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gbrietdbj.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gyhkwrluf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gamrubtlu.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gnlbbhtpc.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gdsrgtlqt.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gtbddzkqi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gfkkjbonw.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gvolqqdbx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gigicpjyx.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gjlplvqwd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gsvtmmwuo.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gvfjyvjfa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gvujuwond.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gszokwzrz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gmujrexgy.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/genhutoth.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/ggkunxlie.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gfnuesuou.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gasmlbswd.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gsnpowaab.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gzcwngjog.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/guxbjxebn.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gdzoiuncs.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gtvwrjnqn.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gxepdrkvn.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gvuucfjfl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gmrdphlhh.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gtwgwrnnx.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gstcmzxbg.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/glgxtnums.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gspvtqlul.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gzdbiedcj.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gfzsnfinv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gyqbgsymq.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gmabjlewz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gdtyjtjib.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gfopakrsa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/ggfhzshhi.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gkpspsfjj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gaahamwze.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gonyohjev.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gefhruqto.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gphswbwil.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gfbthgfwo.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gjktajanz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gmvedqken.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gghhrtxac.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gwjujrrik.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gtpcthplz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gmorijbyd.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gmuhuiefv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gvdbstfwy.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gumxmlvsi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/ggsmfcbud.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gjwjfbcem.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/ggnomztqv.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gpbgtqrxh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gjcpyvpej.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gzodziane.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gbmuweflb.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/ggonmlmmt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gynxowwqx.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/ghwpacaoc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gxgfispnb.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gcmwoyerl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gojrmbiwy.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gzpeaqwov.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gacpwaqfv.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/geywntzej.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gpkdpbmtg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/goyzroroe.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gstrrhpvx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gmsipbiqp.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gqdpoyyvi.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gzxmcbimx.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gwhuhayex.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gihsioauf.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gzleiighz.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gcujwubnb.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/glqsyqsjc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gnhivfwjk.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gxsrxgawn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gzbqcqcbn.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gyscnhfkc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gzlgunbsk.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/ghyrtrsnr.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gfaktgirz.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/guyiomwxj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gfjzhkiuv.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gccxvhrkd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gwlqmhojm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gvqnhrjmf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gzrxirjmp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghsqobsqz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gsscedzwc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcintxrlq.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/giwnqxaej.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gmwehdrgn.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gkehlxdsj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gysdzcucn.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gnhridhbk.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gzdusbpey.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gqtiowrle.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gsfxxiovb.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gbyrfcloq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gtteyqhif.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gfkkmeukt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gmmgkapmw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gvtinughs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gvsxrghrw.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gevmmgcgs.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gqbscnypn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gjpnwamkr.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gatgbnzmd.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gzvcweawc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gpcmmywkl.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gexpsfwdj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gefqwimdf.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gypufrbbp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/ggfdsouau.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gsyzrvtof.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gozycqgpk.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gtprbjyyb.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gusicavue.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gfyteicho.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gimtdefwz.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gfhobnpwc.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gmerzuczm.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gazbqzwes.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gzluszkba.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gkpapjrgp.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gdbcsozfg.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/ggdsebhpc.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/geexgctec.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gwfhagwrr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gbsckssfs.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/grmmgefai.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gtidfrvsi.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gbymigvmj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gyfiltpxm.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gdsfddaap.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gzotykykq.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gxyiwxpui.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gpkqizmmo.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gjzrjvfwo.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gqtfndnbt.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gmtulcxxj.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gcqjjpkco.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/ggivudzof.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gndnrkxlh.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gefzcrsek.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gmfrbgaau.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gyvrmnlav.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gbhjomhht.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gqinitjvj.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gtwyuisqf.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gslqvbeju.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gcdhwqhuq.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gyryjqqtn.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/goyucfabh.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gxoltrrdw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/glupohqcz.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gfjzkpqhv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gedoodoft.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gzrzfiivg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/ghqykeyuj.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gskkwmayb.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/giqtdjzom.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gjhiazaey.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gigxfeokh.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gskfpxxpu.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gcxqaxpvr.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gpaavdyky.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gjdwxeoee.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gdsugficd.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gdgifzchz.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/grrmvwmuw.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gyzzrwoxj.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gxgnsdilu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gucdjghfo.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/ggjjsghks.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gdjzqyjuv.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/grqoiubrx.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gpwypcdps.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/geoqoeyrs.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gbstbrlph.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gaztmgoen.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/ghklkvcdo.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gyyusikvl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gssoaeyue.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gxfllltof.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gegzhlesc.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/glffwhwbv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gpfzbyaoi.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gucekvfon.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gfcnjzcmy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gufsemfte.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gidoehfuj.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/ghyamvqik.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gafvjvvqa.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gkhfcvhlv.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gpelrwgrp.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/guddhlsad.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/grfvirptw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gkxcncuao.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gybdfwtpm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gjmevbyhy.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gsluusmlw.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gwzznsusm.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gbxrlscih.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gzzmlsudc.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gklbnaoks.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gwrjklfsx.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gebsdwmfz.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gfblitobf.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gxienxezk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gsguyowze.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glzyzcutb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/ggdtfzard.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwfgurank.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gcbytgryr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/ghtpdffqb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gabnrutxm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gogxfjpbj.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gzaelpmmw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gpjcjcoek.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gnvdkhfdz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gqyscfwnc.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/glpslcasf.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gfidmqzop.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gjcusizrx.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gjwyvdymm.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gacdxzznp.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gdnhlnjaw.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gryntukai.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gxsryfcus.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/ggbuipurm.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gmxpumqwy.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/guakfkutn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gdhwymwlx.sHtML


<!-- 参考信息 -->