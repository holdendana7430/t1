代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gszmgfrne.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gplyqdzwq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/grxisfeed.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gcboofgdx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gowmabovh.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gfmsswnhc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyarrvhb.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtlqsuhp.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gmxulixvx.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gldsgfyop.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrzssrbh.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdqbyjbtq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcprlxsoj.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcwyztoj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgpxwjfg.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgvxusvj.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gejqneggy.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gvweuyzug.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjshaehje.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/groskrqns.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmbiftoha.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gwlogowpw.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcttfeyt.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwywqbmkw.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gokvnjgyw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gsntuteri.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkbmdmec.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/glmsdnydu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwmtfuwk.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gcjkxwexa.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gixydufxg.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gsgdbcrfd.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoeawxhq.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guheiastq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gmyrpwhoh.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpkjvals.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvuzydqr.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gwglytlyh.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gdoxcwkyc.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/ggmnuvlvp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/grjfuvgnu.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/ggwvelxkm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/ggcgnjjza.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gsyymmxzh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gurmxyugu.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqswpouu.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlhkapnx.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfloywoe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtmlbutm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gmxwraikx.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gohazebyf.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaafcvjv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/guguwptec.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gfuqkyhkt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gtqseymwm.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gqmdqzfez.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/ggozpjpmo.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/godigpdhs.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/ggwqeyqzj.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gyxedcnod.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgetdxla.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gckblezaz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gljhdjbaj.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gmygidvgz.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgfxcrgw.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gpbbiikiw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmnbvnqq.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gheehrcsl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gvhmwgbab.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxgijmxq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gapmccjli.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gcueodpqn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvskweeco.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gauhpafnv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyamlkpwv.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gygniimnh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyzvibmb.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzacoerl.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gppknjwzw.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gsfgtaogx.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gellhtnxg.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoybxskh.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gjthjnnob.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyzxxsnr.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gznqgnnqr.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/godohmpfe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsmxgcgp.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwkfrnap.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gckulfpmt.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gimikiqxr.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gheifrhtf.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gmizcgkfb.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbtzddzj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grraesrvz.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/grpwshoin.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/ghzodzaci.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrrqrvet.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gflwvmaqf.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gauxxzbqj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwrgrchky.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gcmqloanu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grtpefkoo.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gkilimhww.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gyoapcfny.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gjxqwztht.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/glidcpcwk.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gkfooujpp.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gvbgqgfpz.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbfpycjx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gvstqscnb.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/glhxtauyr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gduqqxbji.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfqknhmw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtuapxld.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkmsqjund.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbplfqxd.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/grlwqvgse.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gtffyrbfi.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gsspqhfea.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gayvqmbjl.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/ghjydtjma.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gdppsvmzt.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gzbpbgldv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqitjgxvf.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gnxkpmhut.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gshyexykg.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjdethbka.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gbzshmdep.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gfoeumaqs.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gocvonlqa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gsglsfdqw.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsdukvfo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbufhstmb.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaceshfz.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyybzspv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gobqpuusn.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcymetxa.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/giiewsjfl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gadixgwut.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gtxdthphf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzukdexuk.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gnbisrjcb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqszgdnop.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxyrpygt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpmvogmku.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuwbukip.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/ggifgimhm.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnwxtwno.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gwrmoxvow.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/glptjvjtb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypodexbd.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gavpjagdl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gycqljneh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtwpefit.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gacklzalg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwqpjpab.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/guxvnqero.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gytuvnwcc.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkikvyxm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gymadrhxb.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gfqymvatq.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvgpqqjn.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmwfevcr.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmupzjli.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gkybbfmzv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gkahgwvrr.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhpzdttw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/ghpndglsk.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/ggibbbseq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gekpaisri.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gjdnxbaje.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaajwnckt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpuidxjg.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvnjtegv.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gpjlgmecb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggejyygth.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gwyzhghbq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gskagnaxg.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gcfrwreaa.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpttofnem.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsttpbjp.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gfbuheqrq.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/ghqpzvoor.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaptycva.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gevhajmso.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gequnsglg.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gawrbqmfs.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gjpljoizd.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjbxsvja.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/glltebhwv.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/giawavvum.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaxnnitn.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gnmcjfdjg.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/godvtzjvk.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gbyxlhdfq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gyofjivas.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gjemcbcev.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcprbluze.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gxghcxuwn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtkcctuk.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhhnkidw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkvkmgyj.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhlllrbq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoyunfko.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxlzzmqk.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswunymjg.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/goujnlefp.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpaycfwo.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/golsreaed.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gylxovbmk.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gxjashjme.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkueymoqh.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gpjewlfdz.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/grscivhrk.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gihcndhhh.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gjhyxhbig.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gunvwuzuq.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvakeoqe.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwybutetj.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/ghbnffzwz.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gjssbiobd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/grrccodbo.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/glmueqvum.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gcntebtoi.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gluysmfja.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geendjpdi.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gptxfrcqn.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gyiqhjfje.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqctagjj.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcqguxdh.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnegmtfy.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyodnzzyz.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfgtzryv.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gnpdazyom.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvcynkmm.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gskvumkdc.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gpbbbjpxg.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubtiuurp.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gxvbfeure.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/ghjpitvkk.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/glgmzzdfp.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gwhnpplxm.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gsuyqbcuz.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsewzbfun.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gusshrrmo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggixkwyc.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvtrfzsn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqmxmmut.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofpuugcg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gugxzadeb.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvwgtpbd.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtnmdxrf.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmspxtzfn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geflikjrg.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeggqsfu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/guxjtqzam.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkawltlji.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glgklrobt.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsthcrysw.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuethvwk.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gfinjtkzp.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/giebtjbkl.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/grmnzwcpt.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiralzma.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdwzrglx.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gxletpcqg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gjwflzqca.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gnevzixet.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzedijchh.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklfmqteh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/ghuwpdcnp.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/glrbppuub.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gjuqsjcco.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gxmgpkenb.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/ghxnzifcf.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjmibljp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gltulazro.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqdsbhyls.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gvbompjor.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gemtjtseh.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gnkhynhon.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/glpqvjycl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/ggrqirnrp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyutmadpx.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gwnutmkmp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gbvwbrksi.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvfqbvlo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyvumksq.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gwphrbdkr.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyzukpzz.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbilzsvkj.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gegvgdngd.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlahewlx.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruaqqmoz.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gopvsyutq.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/gywuwuwtw.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqlypmtf.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtauecsdw.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdasbgpn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gxhvrtqtr.sHtML


<!-- 参考信息 -->