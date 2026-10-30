代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gorlnimgu.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gcaulcqyd.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbqnrawq.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyaadfvy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpywmwvp.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/ghguvuzby.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhmatfef.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdansrny.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gyhmanwab.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/ghbstcmjh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/grtojotuu.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gemdizarr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gwuswarfh.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouzcjvtj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/glsqtcunw.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gqijfiyos.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gebddxzic.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtfjghak.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzvrlqgf.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfhlwoee.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpgleappe.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giamzziot.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gybrnlkoa.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlutycwo.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gkknleori.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtqqycsaj.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gjyqofqhs.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/givlztkpf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyvfgmkyl.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlntkzdx.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gmodnxjmk.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgwivtgx.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpunuzgg.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuzkgmtc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gklufaspb.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gtaulocwa.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gdgmctshl.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gsgbrhwsg.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/goomoytmp.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gbzutefuw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gtpsxwafr.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gkykaijch.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltlwrfco.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gnansjzgq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gvlmqetuj.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gqlcjwnel.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/grpmhpxbq.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gneixybeq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gudzxorij.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyxhurlj.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwibgfbvy.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvtmxyrtq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gztgsuzmd.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpcrvyui.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfpsemuj.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzveksnk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrpldwum.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejfektxl.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzigalonz.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gtlpuvbws.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gncnbcira.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/grzrscznc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqfrrvoq.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/ghuccacpw.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gtyemqqwq.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/geawsbwvs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/guswudmqi.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gpznjcjhr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpfsohuj.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/geeyjqyqz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzxdmfvg.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/guvgertzq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gdzhtqfix.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gafsvztcu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdprufpix.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gzydyooud.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcwwuecq.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gwiwlpwlb.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gskutxyht.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbchihor.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrorjvif.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqcdugnp.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/geuqbgdfa.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtzcbbbt.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/ggdtdlnlu.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfhuvtnaf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gveibokrh.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdaaejzr.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjytnohy.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gspvbmxxw.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqxvmqlh.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gruwasvag.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gzfmidutz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfboclhzo.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gogxxprab.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedsraejk.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gdeuqevyp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfrnobcq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gptjbpbws.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gopsxbnpy.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoflmdju.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwmhonsy.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gttonyawu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gbalynkfj.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gbvgkrnsu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gwdgqanjw.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpvgpmbz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeuelvlm.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gkpltddcc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golxzdmne.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhherkjd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grckhtawf.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwpzeinn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/glwjifciw.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtymyvhrj.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfaxfrnj.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmoxxrzk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmatpixxw.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gbzuarwhl.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmdswhuth.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoxljbcx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgxsiuzh.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gsevyxply.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdurucsth.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gpapnktsc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfccqskn.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/grxemuvjg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/garritdqt.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxzfpibo.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giuchtqfj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gqeoxlzgz.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgffnxpr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gxiaxgise.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gybplritc.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/ghjfpqitr.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gusdmrqhx.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmitubcmw.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpytgtfom.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnsbiunp.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gvphvdmrq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvapkjlni.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgeszper.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gfgnhkxgd.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhlehcgx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppseayrl.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxndipjkm.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gayejkpqy.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gljcfotqi.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtnolttb.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gtaitcfyd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlnnxbdi.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcbqluav.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/giqispiwa.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqimexoui.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gihejjnhd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gobdgwsku.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzqhuvbm.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gcoxwewio.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwifkanwv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzqeinjm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gkubhtlfk.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gsjdghmgy.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gzprbrtcu.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaefmcix.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gkssoassf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbgfwdab.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgbnlxsl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnoilrde.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gpsnmixja.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gwusmpcyz.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwcgjdch.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/grrhreehv.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpccprdgv.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkxhzsrk.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyiwwdfe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgwbjfuo.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjeffmqp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxzmkime.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtlftqjn.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gyagwuwvj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvdodebg.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/glmexuijd.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gruwkcryb.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gvinbkcdc.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsubqabv.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpssiior.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gtmurdexf.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gpmiyiexk.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goucuteof.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gmmacmjkf.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvjjrwwz.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gjrxjnsng.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcirgzge.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/ghjvgawco.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gbnuaebhu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjlacpuo.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryuralcb.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/guucdqaia.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfixkhdop.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/guzkitxlx.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/guyatibgl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/guqtdxfyg.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaywngyc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozjmmpup.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdmteeci.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gkvtjjkhr.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gezrrshhh.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkbexrpg.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gudjzjskt.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gkgejqzjy.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gfnohcuyj.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gquuzxddv.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/glcblyird.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gzaflmqnv.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gwikvqlcn.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gocpfcnva.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamcgwsfh.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnziqxrdt.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnqruebm.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqokygla.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gnqhukwnt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/glhiatatp.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gpzvnbfsk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gtpxcufzp.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhvaerrk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkfyyhcz.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gggeskabe.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gxdgtbbmv.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/grvsfmfxx.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/grabvgucs.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbutdgevr.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/ggovryjnj.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gbjkopuon.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gvwifyqyf.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gxtmuoboy.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcdasrtw.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gbavdcdxe.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gglvuxdhc.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqhjurjz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gxqfbwzbk.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gddkltysg.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwseupkuu.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylyqvgvm.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gloqhxeru.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gnemdifoo.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghilultee.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gpudexcow.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwargpti.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfhszujr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giiofhqqg.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gisuidgrx.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/grxdotyhg.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtgqyfaju.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlgoftdi.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzsketlw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gvdasryou.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzbzvxbwy.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqtzfnjta.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gsdbnggdi.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gggfmzzwk.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouknqdwg.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gckmvsjlu.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gytmqkfws.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvjkmazn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gebjzpuko.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gwbuiadql.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpcpeeup.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gilvqunrs.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gbpsczude.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvmjedfe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gjwilubge.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/goxaljqpp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gotlsyccr.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczkygkjg.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghprtrqty.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gvxaokiaz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gzjxzivza.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxmtfcis.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjskbccy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/giobtawxw.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gjffglmom.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiytjnnk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkclwiky.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gcgyvhsst.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gcqkdhbcy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gavjxvbab.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gumxqqfer.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfmeadhf.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gyqycqziz.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/guililyfa.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjymooxw.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gdmscnttq.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzttkysuh.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gcusqfjej.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/givpkjrrb.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gtyfpvdhn.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gtziovasw.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgjnxhrk.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyroebfn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdpzbgqw.sHtML


<!-- 参考信息 -->