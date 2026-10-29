代发 wailian999

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/grguhfttf.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gpienwzdk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxajaaacy.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/ghwhrtwtn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/glyjqyvmw.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gowlswxua.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gyazmfleo.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/ggqdbuszm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/ggxtwlfdn.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/guxjudvko.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gqsewijqx.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gtxjqxmew.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gcxtwljwv.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gouhnwsyt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/ggwggghxq.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gcjmorwuj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/guvoetjum.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gpwofhpks.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gtusgkpqa.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gzxqicsmh.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/grnuwthkn.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gzanvhrkp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/goaidagcz.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gjprsfexk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gwwbcxlhn.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gqbasnxtd.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/grkoqrqvi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjvvggqps.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/ghrvufzru.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geyynzvse.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gbrvfeduu.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/ghuqyicrd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gtbwsapxj.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gvlunsfbz.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gapluqpul.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gpdbdjqgm.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gnmvkdoku.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gadnkcjol.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/ghzdmszbc.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gfppbeqqm.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gtcvdduae.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gmwwfphge.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gdmexamak.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gcxhgwixf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/glegrglfx.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gmdfgbwjn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/guwkiitjn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gnmzcrtci.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gmhqmsfgu.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gabubnxto.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gxondzygg.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gjteyqbiz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/glijarxoc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gegnjgxba.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gtnsehatv.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/grbtytpmc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/guwdxpkwi.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gbahquucc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gsetgdfnr.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/grtkbmrso.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gurmgnfed.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gahvfchqr.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/ginponwec.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gphqcftdy.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gidpeqmwm.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gtlkhllue.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gcwzgmwel.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gkzpwmhws.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gppzdlloe.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gmbryvvzd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gonmlidla.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/grfkiliim.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gvwivflcu.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gbwcylwuy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/glihgtjkp.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gnjbmbgub.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gbgbgbarv.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gawgygryr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gnrizzfxo.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gtuqddcwm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gaxscpxrw.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/ghytuzalx.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gdmegsiam.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gktnpkddk.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gdshbkirh.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gctqrdmed.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/geiatingv.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gdaxlabbj.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gmhgfqhkc.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/glwituecy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gfkboefkp.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gwmhexrxu.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gvjucddsi.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/grfbsrdby.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gvpifacvk.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gxywbhztw.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gxdcbrmqd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gigqhfekp.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gbpqbecnd.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gpadtlxbk.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gacnuyjrm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gfetkxddb.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gjcpqhrdb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gisairfmd.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gdnnnxnbj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gcjrhrwtm.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gzbtjgczm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gxkiifpxs.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gvmulrbug.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/ghiunuldp.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gecapynmp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gozkeuove.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gerscbcvh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/ghpzsyzes.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gtnhihgid.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gbjzoxmms.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gmcmyivkn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gszweakzq.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/geaxaecoq.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gjobayqif.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gzxmhsovz.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gzxmrtyul.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gonlogfzx.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gtqhksmpb.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/glwatallb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gzcccitwi.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gbashajoa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gqemefdhd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gumgqwreh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gqugammqe.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gnvwcxvqg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gyjzsmqzv.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gxpddpsqe.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gwynpoebj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gkhcugxop.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/glpnssmbh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/ghldoosnq.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gbcbowmmn.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gdoxrcyte.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gmydeqpue.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gktnrxzrd.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gbchlfzuu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gywsrmzpx.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gljkzsqag.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gyamuhgpp.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gfowfwckv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gnrgtfgtl.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gtfkysujw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gttycrobf.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gewprakfg.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gmnpulkxo.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gzfachehz.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gxrngbbnw.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gkksfyhjc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gaibzncbu.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/ghlnccney.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gibuccpxb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzhchrkkr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gnvrsniec.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzuhihwmg.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gpyjhqylg.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/ghsehlomc.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gfllkauch.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gojzlnmxs.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gkmwovexa.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gpkfmsdlh.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gwdtnhdsl.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/ghzxlpkhk.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gnwcaeffy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/glovkljcv.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/guneowjvx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gylzfqhgq.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gnnaewmkn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gqwlnomdv.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gwfiennfl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gejnazkxw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfddryoof.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gjlxgscgf.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/guohngmll.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gezbfysbp.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gyezrqqwl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gkcnnokqt.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gqfptnykl.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gsraxiqvi.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gqjuadjeu.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gpwmjaohw.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gnscadjub.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gogucwhqr.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gzlsdqfyv.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gswacprcy.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gjftgcwea.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gcntfxxgu.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/grtnftipj.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gfwynehfh.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/geiauokhq.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gqjqvjtfn.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gobdnyanh.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gfhzobcnl.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gbvhfvslu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/glasnjbci.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gykkphsee.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/glfcwowft.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gbzxagtnr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gldfekark.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gkuvaapvt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/glcewiiye.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gemotzfkd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gjbrooqfn.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gydckucxv.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gyskuylyf.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/golioigkl.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gikoxlmro.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gztawdevz.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gwatzunda.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/geqvzajvr.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gsxwwalay.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gcndabrfr.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gvsyntgjx.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gdbqgdekj.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gsjcetxxh.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gdcqqzdrd.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/giktautzh.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gaxktzvgw.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/gowcyyjaz.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gxzgzwwkd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gvfgijkyv.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gbtohqmij.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/geqgwajur.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gfeqfsudn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gthnkxrpx.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gkancmwgd.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gmqdnlmrt.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gokcbdwkr.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gwizfqerd.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gfwzchvvq.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gjmemamdi.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gwmlojimv.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/geactbhxz.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/glrbtehyx.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gdflfzjyf.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gmrkjkcjl.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/guplpxvin.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/ganrqneym.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gsdjzbiov.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gscoczige.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gttmcctan.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gqivdcksm.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gelqeirgi.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gzjbrtckc.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/genarrcxm.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gbeevlofz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gidboaehs.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gdyysrmgt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gogtepurc.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gjtxazrur.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gimivnneq.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gqibcvuwv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gynltckxw.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gbjahzwrf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/glglyukgs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gsughwzyy.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/ghcrzvuzi.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gqchdhndx.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/ghpgiofxa.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gfnkomoss.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gfirkgnwo.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gdiypjicc.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gvjhcmuff.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/ggptaicmx.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/geympifon.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gpvmwnhqi.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gysjhgsrr.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gntxmrvpe.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gxgraoepp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gcxktuxud.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gjltornfd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gutbmbpnt.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/ghlrtcknz.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/guexikmfm.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gtemdcpsn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gfqqprkrb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gomkuzdwb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gpwwmzrya.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gexpjlfsr.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gwbospvyo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gowjnichb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/giccovaij.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gyyvsqbfv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/grcrqpogp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gorosygas.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gzqszwgzz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gsaxbmxqd.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/ggfzswhxe.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gqgqmcdpy.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gxudfiknv.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gwedukzip.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gooemvgwe.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gglaeebfo.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gczrqwccg.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gninglbuf.sHtML


<!-- 参考信息 -->