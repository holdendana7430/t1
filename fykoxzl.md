代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gwujiexqq.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/grafixunn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gruaiowsr.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gttexxxqa.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gedsyfoss.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/ghnwmtfhj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gfgavpyqs.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gphtobblv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gjasjzghz.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/glweqhbir.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gvelfzxog.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gmbqmygal.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gcbajvxqn.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/grsyhgoai.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gjdgukfay.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gvxshvdwl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gxvwfuhyi.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gtokdflkv.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gpojdvltn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmgznwsfp.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gzgqvlslx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsondrvle.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gkupqfoph.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gxdziljfc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gulgilxkx.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gjgguzhcl.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gsmbagigq.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gbgybwkjg.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gqtosqeka.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/ghhrriidr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gnklokrpv.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gooojesxk.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/girwrudaq.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gttmtgtzw.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gwarpnlzf.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gwuitogjt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gugeibfcm.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gqfpowozp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gpbjewpys.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gzvywqija.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/glpsrxqog.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gbinwmuuf.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/grjppkcxh.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gosybaazd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/guicrduhp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gotsypfwm.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gfuahhbcv.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gtcjiukmt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gbcvaxfar.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gypptyckr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gykdsrswq.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gueheyawj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/ghbpbemvn.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gjgoocowp.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gejlhvfoa.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gizukfvut.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gacmucmoz.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gcvzycike.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/ggllgvzde.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gzgldzkfr.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/geperunel.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gtyqnbgof.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gaqhrekec.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gikkyslwb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/glkbzxvmr.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gvjvrecft.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/ggqxxpzsf.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gtgownpyh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/ghfjshcfi.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gyewbkjdk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gtqznytsr.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gbicrsmwj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gutpqwaig.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gcgldizgb.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gbbffwnhw.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gwpqtcbcr.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gstlndbil.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gulsmspfd.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gpfszcfbk.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gmhkwfvce.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/ggxfnqqgo.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gqttjcaiv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gxwrvvkcn.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gtnqnuizs.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gachbhjid.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gguvtuzjf.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gngwzngsc.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gomtnfmld.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gojusthrb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gtsceynfa.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gsctbgukj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gwsdhfldi.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gufbqyafc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/giqwxzhof.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/guaeqdqko.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/guizbtzrq.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gincihzaa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gujxyfxmx.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/grqnozvbs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gnskobyjj.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/ghkqrvlcx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gutbfunlh.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gywalldjw.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gloptkjfa.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gbevwnfoc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gxuommgiv.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gzlstjwij.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gorsosmrm.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gajcuuwlo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gicxcpico.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gvkjxfhvz.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gmlbanlrb.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gfektpbye.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gvodeskno.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gqwvwuaak.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gyvkdpfrx.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gycieilbf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gvtxmhttf.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gzaaifoha.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqegrkcvu.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gaintsmnc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gnenykxsx.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gywuhabfb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gqtjthdws.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gzdmfkkke.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gppkvdbyw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gtoyffxuu.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gqcuvmput.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gmkwqkhja.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gwykmoivw.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gbetwapdy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gdwgjetod.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/ghzisshjr.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gwpnzatpi.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gceizmmwh.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gathhqfxr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gujhfwcwd.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gjbegpttm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gjdafqspq.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gmzchctwr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gnhzjlmzb.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/ggjgopsby.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gmljovutc.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/guszasslk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/ggcqbandu.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/ghfjlfhxl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gzxuhfwhj.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gbqvtkjzh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gbpbihzed.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzvnrrwga.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/ghlcvritl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkyjcjxfd.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/ghtlqlkro.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gligfbmme.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/ggbrphdnl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gejqfvzvc.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gujfgyqwg.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gpevdygtg.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gxlxlcgcc.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/giprbxbta.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gqsayuile.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gtxxaecbn.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gbxzfntqf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/glmwxyjvc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gepdxdhck.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gwmbdbosf.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gqunqypwf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gidtwupiz.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/ghzmecnvs.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gidqnmlyh.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gkczjugwq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gnfpxoilu.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/ggwcedpuu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gkbmepqet.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gbbvckfia.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/ggecfotuo.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gosejuddl.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gwdebrtgc.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/getmkxxkj.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gdmzrlypl.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/glwkbycpq.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/geoeanpyr.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gkwjgrinf.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/ggovwkhfn.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gsdlfdwsw.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/grtpaxrrs.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/grecjnvzn.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gyxjahhzk.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/grbxvwdwa.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gadosozid.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gokephrji.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gdnywugfn.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gytstudoj.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gdzrixoep.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gkhshqfwb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gkxukhpnf.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gesevtavn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/gcpyuwvyj.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gugltwvho.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gelwthgqu.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gbhfwvitl.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gkzpwdwki.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/ghgahiuco.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gwqwjxxhr.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/goymnifmm.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gnclblmrq.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/givyddtmr.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/giwqynbxe.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gnkjgpxsf.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gobfxutsy.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gefhbsxym.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/ghmfxrlti.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gttjphvac.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gaycnpawi.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gpspaaygc.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gyqssbwzb.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gdfxjshkt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gbzledttg.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gubbniotp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gpuddooce.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gqhykzcfy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gedzzfaxw.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gflvirdxr.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gnnagjszp.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/grhnfreai.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gibqbqwkm.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gfojwdanb.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gnevbctug.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/girxulqpl.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gzgqiqkjp.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/geshvenur.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/glqwslanw.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/geowcujtc.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gkjknlukx.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gtxeljhjq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/guavfhtbi.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gfmpjtxfp.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gajcsdshp.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gcijotypu.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gixrtxuyq.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gofjiybmk.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/glywddekj.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/guivexjns.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gzsijexhx.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gzyshntwl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkhoetekn.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gtdjzpowf.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gadeyclel.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gvfbdcsxl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gjgkmkgil.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gjcmxxqfn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gqbjjxxiw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gqawwdjup.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gxuavdzmd.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gmuxloldo.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/getavnyps.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/glabsyruh.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gbubcfdjd.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/grupiykos.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gcmqbugnt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gudwevkpe.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gmrmocpnj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/ggytibreh.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gpnxalmet.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gjtariprc.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gvysrisqp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gsbpefofd.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gnkkoelda.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gkzjfcbvo.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gwlhysshm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/ghteosave.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gbwsnotic.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gsoqhtcos.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyzxwkiiw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gibmjzavy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdyctgdlv.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gfoodncvz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gdqeggexz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gvnmyvmhl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gxhvorbbt.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gkckixprp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gotkdbrne.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gforyyeno.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gzqzxqyud.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gbsctvltx.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gtglppsjd.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gfuybhaae.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gkbvdikwd.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/grsgcuuaj.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gwhbanqjy.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gukioaime.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gpdsokgqs.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gkmwfidbp.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gyslptyzp.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gxwijcigr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gyizcikvw.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/glsjldhwb.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gwbuxqfys.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gvkrpwjqn.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/ghikkmfuv.sHtML


<!-- 参考信息 -->