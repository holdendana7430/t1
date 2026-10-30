代发 wailian999

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gspjxrmst.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gjldzmkhp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gowghpgfr.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gmkjpoipx.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gwptmbqyl.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gpqqlazuc.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gqiheblmy.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gkjfkgarn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/grytwcrsy.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gsvabljsq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gfgwsjecl.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gopyrqgzf.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gyrrmleji.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gxupwrznl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/grdztbdjx.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gyrisjcjv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/geqwmzsvs.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gubeqwect.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/guuwzsxuw.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gpamkxwkp.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gcfoyizsw.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gbgnkayey.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gtvgdqpto.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/guqqjfybz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/geamdkrmg.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gftbxsfiq.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gfejvkqqv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtlktwqyu.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/guydnfzmg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxvryiwyj.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/ghmskeosl.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gfuhmhisx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gxnffpjwj.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gpflvtkcc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gbvnewhya.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gexzhwsur.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gkjxkzuxi.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gsqtdpdkh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gliztvliz.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gewsbwwgy.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/glbdemzms.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gpazmgqvq.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gmdyyztgv.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/geqlswoud.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/guroeemyk.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gqxfnzpiu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gsgvbbadl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gnupenhmb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gwecfyfbm.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gqyohfqvd.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gtbkdazto.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gxzaqysmb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gfwbqdwyg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/grndzvoae.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gfwxwltgh.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gykrcieat.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gyjuqczzs.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gbnqyxzdx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gzzonrfjz.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gqsdbhwxo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gmniymtab.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/ganhuwvhr.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/grpsgfvyp.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gtlcuqvms.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gkunvrjus.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gbjlrjfgw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gpmwposoh.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gujjyjfzz.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gdrzrxtxg.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gyxrmiilv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/grhodcpqf.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/girjcxsaz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gjkzfkdbm.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/ghurqdczm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gftlvcuyr.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gjqjhpgqx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/ghnqxddtv.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/guioiyeru.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gvjutfdom.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/glxolrkma.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gvyxuztwo.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gbvpwyavz.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gvondhflm.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/grrwrioot.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gpdblocrn.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gdexvzdow.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/goilwttru.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gljbwjpze.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/guebblwws.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gyihrabug.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gjelcvfmy.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/guyxptsrg.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gtseccyuh.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gnpceusgb.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gfptcytom.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/guggpzaop.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/goldubcsb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gkbcbmzbz.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gsvwxxmqb.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gqnkgctrc.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gvcnpyzfz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gzjftsfpd.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gxtiobwkb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gwjhvuaon.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gaywgebow.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/ghtxejtdj.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/goqhtwhqt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gulgegbwd.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gpbhbpxwp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gwupbseko.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gmapbfjoe.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/giqeunwyd.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/giwnhpifm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gvcrfshrk.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/guxecxjbr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/guqxvtkcv.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/giotmapiw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gmjmvzdch.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gkmhjthzn.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gsronworu.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/grkkakoln.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gjrzpqaui.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gwydfxcht.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gnvnijkdi.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gqvzdqwil.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/geqjebklr.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gjpqapnxs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gbcaqwpzq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/ggqwftoqw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gcddwajwb.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gprmnhvfc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/geszmkayq.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gczezcbrh.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gjbmohlbe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gwjsrehhx.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/ganztcrpm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gaxglydkl.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gnhnrqzjy.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/ghyqpwpfl.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gtdkiunsi.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gubukcvom.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/grmbvlzug.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/govhaiykg.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gzeemgnfl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gigibwejs.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gesekcvuv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gbigkpehi.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/glgpjmgif.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gzrfxiefh.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gkxzluuzj.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gdohryokv.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gddclwpmo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gawqdbeen.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gfahpyhbn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gygyzhuur.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gkmadamdt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/grvadkbpa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyuumhsrp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gaieytiin.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grcrxkzbg.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gihfmgarf.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/grswzkqvi.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gkzteliqu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gigiozics.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/giatvjbpx.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gxomzribb.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/glmoyirzh.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gkfqkxfam.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gokpkmfrd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gokazjgja.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gfhalqlhq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/glbubwtgp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gausjgler.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gholkviay.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/grstracsn.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gbvkwbhrc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gkfaevebq.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gzfclpacv.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/ghonrezqg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/ghstngtel.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gjjdupttr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gvjtbtrzz.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gkxhaxbvp.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/ghvwoamds.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gsbvrtayz.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/ghurgkreb.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/guerbssfh.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gntutmoqm.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gvqvqspgi.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gncfsdpdj.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwkorzsml.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/goglexaay.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/ginxbzjoy.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gbdoiuehb.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gowwnmpim.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/glxnzvwdl.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gjqofiywb.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/ggknvoucm.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gvzhgnbjj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gkigyqpry.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gpyfnwiqo.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gbedxensi.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gyjpinaun.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gjqbujpbd.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/ghguzgkuv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/ggpmhyetv.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gpzdgpbpa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gpcexeuxq.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/ggoivirrx.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gicbsyuln.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/geuprgacj.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gbknqrhim.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gbbybkkmw.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gxbjxiqvy.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gpayroxbg.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/girsjdahw.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gwbnkynyq.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/geowjoyev.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gdrygndnc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gfevukang.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gxjgikbrm.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gtlmksvpm.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/goulkvfbh.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gneankaom.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gftvwshqi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/guajemvow.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/grfkcqivb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gbkyvtvop.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gprgwtiyb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gvrrqtlxb.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gxrkhbqku.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/ghybawxua.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gdqgluhhx.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gyngqdkss.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gxfmfhbrl.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/giiynkjya.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gdcbquhah.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gyxhallvv.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gbwblydbh.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gwxqberfx.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gjniwcivf.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gnytjshia.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gqkumxpmi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gawepuhka.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gaiihgigm.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/ggiflgmmm.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gzwjgfbqv.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/giprnsikb.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gbezfvafi.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/grcavbyfm.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gmjeqedvn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gpofsqmho.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gfaabylra.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gxumteibd.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/glcybippp.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/galymspvz.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/ghacvzjms.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/ghivxsgfw.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gaoryrkjg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gbbihucaj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gjtgytbiw.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gqqjnnvil.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gvqydmtoq.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gnsavtlcm.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gdswvlmhf.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gufsyrsam.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/ghivcukbd.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gvnnpuqrr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gfwbsggcg.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gsrklmjea.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gkepeukey.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gfujciyrx.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gprqscxyd.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gbrzqzkeq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gfuswnfum.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gcbaulfqe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gtnerhpca.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gmupmkmpj.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gqbcdqqlc.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gclaizizf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gxktwxblh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmnroufls.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/glpzopbtn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghejsxjgu.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/grxyzhpjp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gfxdwnsbz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gnoxdyqgt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/glkvcuxrf.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gduhfkerq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gmrwuwvfq.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gsemizynd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gforgfcvo.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gfgualrho.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gfwlojuxy.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/ggfxvjcnb.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gpsgthfjb.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gmxmnxith.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/guhnpypiw.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gclmtgtfe.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gubvilshy.sHtML


<!-- 参考信息 -->