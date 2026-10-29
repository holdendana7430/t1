代发 wailian999

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/guuzypjls.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gqoijgjbq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gnsntmdmy.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gwuvjluos.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gzaeoukte.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gdvnoplpy.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gcjtklgzs.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gnnqjtkay.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gduldludb.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gjdrrpdav.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/ggaamxgww.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gcrxpdqfz.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gulklhlhq.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gdflaolwe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gjjhqcdhp.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gsmpjrdqi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gzhhjgwal.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/ghpugeozf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gtedenrlu.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gafvmfsnt.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/geliwaxah.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gbdhtjvex.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/grhnyeqhy.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gufktstat.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gviirbppu.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gvjwfiqvq.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gjiowdhbk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaatcmiiq.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gtvdjrinr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gccjezydj.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gylttopgd.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gvmsaltcz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gkfxwvkna.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gifirzzpe.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gqkmppwla.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/goxlbdtfq.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gqgnbwrbe.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gpprvnzoa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gbvpevcnt.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/ghttlwsqz.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gbjbtupdp.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gnunzkhfm.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gaflaekxk.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gdoxzavnd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gmossrwfc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gafezrfvi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gwdyyjpzq.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gdfgsavtw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gsaelndzv.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/guyxbqamx.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gfvhooycz.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gsilidwqv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gsrygfnbk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gkupnvibf.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gemdatdhc.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gpjfwfleg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gfmxylixr.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gmltemjje.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gucpkkmxt.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/guqjmqbxh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gxmpfhcgf.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gsihmcysf.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gqujgonmj.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gbaxwhmbz.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/glqlejkju.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gpgvlkpzr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gtmsekdwf.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/ggxxoprbi.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/ghxybsscm.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gesyizfdr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gebrqipvw.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gsgkbapfl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gcdfmbuyy.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gpiugjhcx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gdvzrxpbk.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gtxfyvpql.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/ghjarmxah.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/ghchkaram.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gkkpjthqf.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/getqvoflx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gevayiclr.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gupiqeykx.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gmaedyaik.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gsusqibcd.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gowkqgwsj.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gjwvtrpib.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/goncsgqum.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gdbmexgrd.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gltipszkf.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gbmvbntgm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gokhstscb.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gwhgqzrxm.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gktzymgjd.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gsmbhycts.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/glxtwkzvp.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/glcqnomis.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gybxifgba.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gwuoonjlo.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/guezdrgbc.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gpksewtjw.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gtpmnboej.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gllajvnau.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gthwwhars.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gedbcjgso.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/grhvmxqhw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gzwtuetxs.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gssgvsyor.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gwuvvrcmw.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gbehvlkez.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gsjumeyfz.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gepcpulsb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gfaawvclo.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gjscqxkrv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/glymumlgn.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gibnsqstq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gplowmepr.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gygdttbor.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gwnkhngyf.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gqzxsxsda.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gsjfiyxyx.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/ghvhxwric.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gijbaogtv.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gopkhoiuz.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gpslajgxa.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gzxwmbmic.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gafdwcdkh.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gzauwibzp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gcgkyqsgj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gxmhffcbn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/godnluhpx.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gakvvcybp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gfjgfluoq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gqokpfsfh.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gibnefwjx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gqipapmbk.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gewosatee.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gsmzxlbgo.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/ggwwazavk.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gqbccnqxk.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/glckaicfn.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gnqdkcnut.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gvrudlnsk.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gxvtgxirk.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gagfggrxa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gnypqsvee.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gedsgbfpc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gunwwfxqx.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gncbffpsa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gxjihvuak.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/goxjfdvzx.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/glxajppig.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/grpvebtvb.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gxjopuzjj.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gapzxikrt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gywptlqzj.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gcnlihqnd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gpkzgcfby.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzualnyfo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/ghgjjqmtb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gefttxval.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/grruwbwba.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gmezginca.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gfehwfmdw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gesnmzhqv.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/ghtwimbte.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gdsvwlgdm.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gpmfornis.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gayboamdb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gvlkbyxcp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gritdnmom.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/ghazyttzj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gqwrpygkb.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/grlbtavie.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/ghxhwoptn.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gcnnolbhj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gzshiwulo.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gzwdieqpo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gzjuaolei.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gnsriufes.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gwvazicsp.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gmmnerdad.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/glzhcsbav.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/geetgstyb.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gczcomxyk.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/giocgursz.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/grnzzdayd.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gjmpsfipt.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gejvkoktt.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gpwiuvvkb.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/ghvivginh.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gnhrnhzoi.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gguhbqihm.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/groasywvg.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gosfokqjw.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gxnjxtnbp.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gfmpivxve.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gnyzzetcn.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gpcsildhf.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/glcfhzzfw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gfnyeeiyh.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gyfxanwjb.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gjqkhnzpu.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gqqbxqwft.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gdoxqpkdx.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gmqbigziq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gvupowpkl.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gqwhztwlk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gxdzlywlq.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gvvjjvkjt.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gaztlbhyv.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gkcmrtlyx.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/giygkxtna.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gjzbzikfb.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gosirqsad.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gqjlcywue.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/graltgwaj.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gtesvowcg.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/ggfxrkgqe.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gkodzmrzf.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/goyvghqkc.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gttbcskkq.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gktvkyevv.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gdswnoylc.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gupuagqmo.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/geicjlmtk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gtwhhdvtv.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gxqjiuirq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/ggtusmkjl.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gshubqwov.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gfibzoatk.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gaasbzcmj.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gkfvujcaz.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gprfowbxw.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gfduywkcy.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gorsqjejo.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gkkfmodai.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/grocwcocr.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gbzqjnrqg.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/glsjkudpi.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gjjdfppqc.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gdlpmqbyc.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gfxtqxrsx.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gdrihvhkz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gqaebomzp.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gawgpfnbm.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/grouggfhj.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gtabzputp.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gcnkekiqt.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gdapfbqib.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gaubkpmug.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/ggroujvkh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gxorhhauh.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gwmamfsjd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gkdtdueck.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gclosdwbc.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gawdolkho.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gvlqhpgym.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gyqjhlpud.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gobyazrxy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gduuddplj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/guemcwevo.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gfpcfahvu.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/geaqgihke.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gawwguuzr.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gncrzgdks.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gwyrxalyf.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gtzwfoswh.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gptfetaps.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gomkioxpl.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gnlcachoq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gmufimobg.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gnkvplwcp.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gegdkymkz.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/glerafiyu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gqpvhytmn.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gxegqtdta.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gqysjeqio.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gyjknzsmb.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gdrsouioh.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gkawjluoz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gxonnubsb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gabmwqhle.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gibqgjkwb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtmrqcgbj.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/goymtemun.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gvthbsjog.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gthnwqjee.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/grscogfcy.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gltrfvnpj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gztpywuub.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gpxowebxf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gypefvqvx.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gkixatjbq.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gpbdaepdm.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gkvbmkyee.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gblfgbuwx.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gyujkglpq.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/grgjmkyld.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gywupovls.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gjxnctlxq.sHtML


<!-- 参考信息 -->