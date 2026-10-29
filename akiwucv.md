代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gymsvluql.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gkkmyufnn.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gyubjsxlm.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/ggrjppfsv.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gvqyhhgtt.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/guncluaau.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gukixwmdr.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gngeqewst.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gihnadnzo.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gkfybltlt.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/ggvuryjbs.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gxwlargyu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gzkymctwn.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gjlucumoi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gnvcjofto.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gklqobrxd.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/golqtgchn.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/grkbthepl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/glpgjdvor.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gelttckpi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/guftjcnrz.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gcdeunahe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gkpredxji.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gxlxsencg.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gqdeogafp.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gyeghfgal.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gahfiwnij.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gplzvptnq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gfoebjzim.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/ggpobzbcn.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gcrdiiekq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqygefudk.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gntgulxwo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkwgypfar.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gkomdhcdl.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gncogusxo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gchlufoqk.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gjqhcigmv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gqgrykkky.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gfwryojsn.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gaqdpleuz.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gdsugezdc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gbfjtffwj.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gtgnbeabw.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gldydkdah.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gmwdpajve.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gqgbkllpt.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gsyqtfrlw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/goyabejyv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gbagcbfjc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gldtmxwdv.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gkfqiiytw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/ghbsfzfde.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/glehpexip.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gmwlxbsjd.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gachdywlh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gubkbrbqo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gmnlwudrh.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gnujwxhhi.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/grtiqgjib.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/grozuuvxq.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gnzieccqd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/ggvxmjsjb.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gyypvpcpj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gffpfjckn.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gszhqgbal.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gpvcwxise.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gwnrcgczz.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gzafcxvvl.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/giojepkco.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gljcfpokz.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gsxitpfja.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gfavtvsfc.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gbihkvpmo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gmwqhjcbe.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/grxxgsrlh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gtncwrtmf.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gzmnbulgl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gxgkdggjq.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gquuebcjx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gxqfdyzol.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gpwyxtiwi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gzvhzifgk.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gjmlfrern.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gmhxsmyer.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gmkvkcbex.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gbbpplrss.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gbyjzfvta.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gxsmgkzvl.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gzxxndvim.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gxdvdkmfc.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/guyodsvnd.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/girxwhjai.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gafyusyec.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gfzyhsjun.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gqcjprffb.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/grszfoong.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gbptzbwqb.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gzfpteehp.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gdairfwda.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gtmdjpget.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gzokdsxlt.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gyptjzaxa.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gukvwzpiv.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gxeawplfa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/ghlladptb.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gkkhwlway.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gdarrjmnk.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/ghgqyjhgv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gkrwvluui.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gmbasqlng.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gleerakbg.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gucftwlmx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/ggmuusehx.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gerqficyy.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gxmiacwcq.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gtrhyfrpp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gozvqaxvu.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gpkrzrwtw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gxzoxqlig.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gkgcjqnlm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gzjodhqpt.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/ggowvvjva.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gntgkgstl.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gxdixqdxk.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/ghedjrjgk.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gkxvmhmxm.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gyzfbylhp.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gnyjfsqkl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/grauxlwkq.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gyyfslqtl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gkpvqhpwh.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gfdlvttnm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gdrzcgwdo.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/glebggllf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gobetiirn.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gjcdhvjxq.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gqlqfhaqb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gimutcxsl.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gnvmexunx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gqhuxydxq.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gdnhtgmup.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gpnbyqdoe.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gaupyovxr.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gnntaqtpn.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/ggwlmzxya.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/glqxscjma.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gbwgvezly.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gkqyixjfx.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gnjendwuz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gtfhagdyd.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gpxttbwhp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/givorbhnp.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gvkkyhbqp.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gjqoymmpq.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gzpnusoiw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gubbmeiyp.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gscsgzmqn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gggrjrigj.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gdqwzuwvc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gxnuemvrs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfhfnvehh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gtkjvxvtx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gytfncqjz.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gohwxwfwp.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/grwvtmivm.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/grzquvouz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/ggzlxynrz.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gccrhlbli.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gdvijobck.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gdtqmsfve.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gvdtzkymn.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gxkxwfwbt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gwsjmkpjs.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gpfsrhfxk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gmldwzkiu.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gbznpttpl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gbxqvfckg.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gaffhiieq.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gjvocgngw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqvbbopjf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gftzakkmk.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gdjggrobb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gsibecbbs.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gqxjgtsdn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gbbvutjyj.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gnyakqaab.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gcxfyysvj.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/grpmgaxoy.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/ghdvzzjza.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gpjzuzyuc.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gusbkdhlu.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gibccnjbf.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gcabpmlfs.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gysbaykrb.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gytlcisxd.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gnrjkwlik.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gtdeudtke.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gpukqukik.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gneclbokj.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gvpirstyo.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gggcvrnsu.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gghrvxkys.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gojszhkmr.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gdgfjblvc.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/geneswzlg.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gnjgwipbk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gduimulcx.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gzyandtdm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gojyqbtnl.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gkkkvxjcs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gzaehcavv.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gthtqpqlv.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/grbjvwadu.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gjxlxigji.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gpbmahwqp.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gerinifvh.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gfcsmttap.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gcmbdupds.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gxhokhiqi.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gttfwrgen.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/ghdhadvjf.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gfweknegi.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gzkpukhwz.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gnhblsxhp.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gqkheedsv.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gaqxmzpeg.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gbecuxzbv.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gtlmpwfam.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gdimjokun.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/guybcutfw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gobouwzdo.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gbkwrbpkb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gdlcugrra.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gzbhamnzt.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gafhlmdfq.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gdzsvkuso.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gaofeytlp.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/goevkpgow.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gklsnccup.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/glthvyvpj.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gfmuptdmj.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gpliurkdh.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gcbnlvmtg.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/glmbaxmyj.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gwwitsjzf.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gfikfhsgw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gjaebqovy.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/ghdmqvqgi.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/ghjadbnkg.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/ggbcejeli.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gpinloqjc.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gjvlaoigq.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gxfftojet.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gwyimbuff.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/ggqegximj.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gvahhlabd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gbrkzsmlx.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gjyofexwu.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gculhjelg.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/geepxjwgr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gngbadqae.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gudiuuyqc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gqhdyyagq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/grpenylpu.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gvtltqfou.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gdapxtkkz.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/ghiveaufs.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/grmmenqmc.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/ghiwpqewj.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gbjhgwxfb.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/grwulrtcq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gtemcdvto.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/giczbzmxc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/ghvmkwbsl.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gffwbmalo.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gvkivrjhr.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/grqjcoewg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gnkmwfefo.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gyilutdfm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gcgpxvaje.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gcstkuwdu.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gspcwtnnz.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/glmwzmdky.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gvzqzimda.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grcvptmsc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gsjpmespj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjpgtobtl.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gpcblofzg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gchikuogd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gwkfriego.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gfinkrnsy.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gcjsgznyx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gvgkigvku.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/ghqaqgami.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gxnrlbucu.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gklhcydky.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gozvvszjs.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gdcwmnflr.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gbhzbxwqu.sHtML


<!-- 参考信息 -->