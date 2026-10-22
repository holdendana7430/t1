代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2vdmrrkvu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2cmagatrq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2zqxdokxa.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2hgrsavae.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2dgbaxsaf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2isejgrck.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2iyoslkon.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2gqytcxen.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2sgjyfigx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2elwapceu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2gotdlgph.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ntylmsax.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2xeuwghgt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ncivafih.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ubpszvem.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2unxbywmj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2fqccddhv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2bnuhruas.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bdisuanc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2xanbrvch.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ehblnusv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2bpgbirtr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bnrvqhbf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vlfmklgi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2wtxsirqj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2vsquwpkr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fxqqdhpe.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2emccnbkk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2pqxkucfd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2nxazafrt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2yrhgdjju.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lgxjrmcx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ilonqoyd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2jewsznpx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2akvwhulj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pcepdklc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2otwogwlz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbhbxvxw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ifoliapo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2kelajtan.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2nghrfxhw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rztkrwid.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2etzadzii.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2qqptktqv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2nvwhggkk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zmwxczqm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mnjivljn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mjbiasam.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cpuccceq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xwjpfcwt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dmstzixj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2xqofsnli.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2speosasj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2kldqwqnm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2envtgady.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2dumjaipf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2utduevfr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2kkanvxjm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2syuiexay.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ruvjcopl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2gyksjdfg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2vfkrrowi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kcuudrwv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2brfbvyku.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hhjvobzh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2facgmeab.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2cuachhxe.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mmjucqhc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2hzbwqyqn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2fymghwls.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ivbmpgxv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2vbicxpey.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dltjdqqa.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mripcrpp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2wykavanr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nhyutxrb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2zupusfnt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2zimdupzq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2akgoyuda.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ipivanih.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2feunwdms.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2todkbadd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2pdsbalrs.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kvudlhpn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2qflprtwq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ywaxqbgc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tvzfjmxt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2gvqkhzbe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2dofeggtb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2tzlsazue.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2xgobwmhu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2szgwyaja.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2akstkbfj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2iweqbgpz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2boupwvpl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2yddjbnmx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2drleshlf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2rnmdbgtd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2aixsnnkp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2akxyjswi.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2cjooybtt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xaoobhql.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2pjtwwuwi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uzqbpfux.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2xowxploc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yttkuhsf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uqwuedvm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2zrxegyvk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2eahpuckg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2srggxsqd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2vazhfkmb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2dnfcatdm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2funvpqvz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kcrjombq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2alsonssc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pjltnmwk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2dfxonzef.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2iwphrqjv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2qndiolhc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zfrxfhri.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2iiltmxrp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2dwfuevhn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2sxbgcguh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ucpeoaoc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ajvfiygr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2vrnuztow.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dclcrqhz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2oqkkzcun.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2kriknqjn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ezntlxsf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2zilnzzud.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwsklvkz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ttjgpjxk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lfgztzcq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2xbdxjqjj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsmbvzrv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ebkkznef.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwatxknc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2enmfhqzo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2skylbzfk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hfwcfxxp.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xhinyclz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2luawapva.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2rospibhi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ezgmxpni.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2wwgbmvzp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2oxbfoovk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2byffnine.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zrexcovl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2tusyslcs.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ynlmgayl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2qfqfvajj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2uctroafc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mohxhtas.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wgwbgymt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ruywcwxd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2iznstvcz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ishnyndl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2azzvwckg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2tlchszsu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2lhbqtluc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2jmenffgn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2woaxvsjb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2guhfhqtr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yzmpuczp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvhrexlv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vdqiknwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rcracnra.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2venrpsly.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pynmrvyh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ctivjemq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ilmubrny.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xyzoyxgx.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hcybebjo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2cagjjzqz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2kintdivx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qyphregt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2efunmsgv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ohdfmilh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pitgwxfg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rtwkrvlc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xydwjffw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2eejexklk.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pmtycgno.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wgjwbmxu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2eajoxdan.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2zzmlrkkr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2tzbgpcif.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2wcdrwina.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2igehwlyc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ilkzcedu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2arxpenju.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xpholofc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ahezcyom.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2iggqrbtb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qrvwpblc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2dsdxmklx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ippixllp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mwxuchdz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rpdarbba.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2zxdddhgm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oshdstai.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zlfsdqrg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ebxxfugq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fjcixzin.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2eiimuxhf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ipryjkqn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2jeiolxdq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zsrlwapj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2jiggmete.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2znqmufxm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2rnzvnagl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zznupqhm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ybgesprh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ymmdyxkv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fuaeywqm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2edgtsrmv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2pxvwujzo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2yfmegsip.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2lawbjifd.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pwoqeljl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2nlydcntl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2iymteecj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2febynlqs.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2fvukxwav.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2uenurscj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2xqcessgp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2mxjsvahz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jnunkems.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ukkdrzeg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jgcdrnwh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tmmvsfiv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2elzisobf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rfmmickx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2kfiabidu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2gcvmlnev.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ufykrjzm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2euytldel.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ahwhbswf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mdqtuecz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2zutmtiad.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2oibmigqn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gzoqfroj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ooeuzzct.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ervzyjhj.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2kfsatuwd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2omjhsypl.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2knhomfxd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fcocurzk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2onugdpxt.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2nyozbexl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2flgalqwq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cmwcqinx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2cpyvyjxk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2tvyyeasz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2qiipwgcq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vbscusut.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2brubovie.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2nvmoeoae.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2dymzgedq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2jjbnwzji.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaetrfcw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wgvafjjv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2gtkdntzl.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ypvtlxdf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uafmzzkb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2syicxszy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2lypsxqwg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjnwkwgk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fkueoebw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2adberpfc.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2aygxtdmx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gtscpihh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2byoxicmw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gqlsiahn.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gxvrntuq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yynyuhes.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uxddjcin.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2drqtisdn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2lfrqabwl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vuuqabbf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qbszksor.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2yjkvgony.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2kykyyeqd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2prwhthjb.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2tyuccpky.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xbxwslpx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2rtcaejxf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xalaidqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2joycdsgy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2eagczxuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljtregih.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2niigapwg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2kmhfngqh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2kkgusbkw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2irzlzpeu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2owrpqfwr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2bwtalrrx.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2iowiogwr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2zcumwlwt.html


<!-- 参考信息 -->