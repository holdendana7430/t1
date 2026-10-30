代发 wailian999

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gubkglcnq.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/ggzkofymh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gtgidvutj.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gvaasuplf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gvtqpdybr.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gfcjixfgd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gghblrewu.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/grebnszcd.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gkwduqkeo.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gsxxmhsca.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gkykerejp.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gxyshkaju.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gbmnlmqtp.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gzxhqgzlt.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gnjjkqwto.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gstncskpj.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gjfkvaxrq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqpzvrivc.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gjltlurgj.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gwnzgctvg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gqhyjdnof.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gaaoesaiy.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/ghboihvnd.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gmbyormec.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gdqhgymam.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gerhzzvnb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gqekjvgxk.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gzbhyrqmq.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gfcieuknn.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gbqeorzmt.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gppfjrbdv.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gxbotvnfm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gyhjurikn.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gezbmgshd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gfmhuferp.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gsfpbvnjz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gydnffdem.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gofemfodl.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gffsvivhu.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gtskyptet.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gmlphgsdv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gquiwzmco.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gnhjdyssl.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gxfmhivtt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gudiyiplf.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gmmootedn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gtuzjrpmb.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gtiyfvvqq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gudqvadkw.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gkyutyuse.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gbxklqkdr.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gwhyvapoj.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/glutqgbqq.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvchqzcsl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gfvbjfzai.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gpsdcvkhg.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gjavomlau.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/glthfftal.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gaydanslb.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/godpfnvmz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/ggfzlenmw.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gzztzrank.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gxvductwn.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/goalefope.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gevzjhvli.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gkngrkyai.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/grkaaiyvt.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gmsskzlkm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/guetjtama.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/geigwcfcl.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gkrzuurrr.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/grefptbvj.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gzxwtvjlc.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gspsovkpm.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gjyfmbcvy.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gtaqqfugw.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gpezvdviu.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gbduilemz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gcwlabwaa.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gnxbqadzk.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/giodllium.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gvjxllqpz.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/giazpabbz.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gkrpoglmd.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gojixccym.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gvouutsbw.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/govjpwdbm.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gjdzgmvsj.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gftlxokow.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gyntsomqt.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/ggltdfryg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gtwiiducv.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gjjnvuafu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gfjnnpmjm.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gvmhrvvau.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/govolztsi.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gpfkidgdn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gkvqrurwj.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gtkehadwh.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gqbolfrbp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gscxbauei.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/ganrrxcei.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gjavneheb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gpaxmyusb.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/giappiknx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gxgrifycn.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gmdecxsom.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/guckdkupd.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gjzknqojg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gfxnzztpz.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gnutzqsms.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gojnhlfma.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gwxfcnumw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gaanzchgk.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gyvwcccwq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gxztqukom.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gtocbdbss.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gyubtxujn.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gxakjgcuw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gwpewrxzn.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gqzzbypgg.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gudquhxna.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gjeswmgkc.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/ghufggjpv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gnyiimyqu.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gsulyrzss.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/grsjlznsd.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gwxdkffku.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gczvdwshg.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/goemwebpu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gjdhpvbbh.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gvhfvyhlq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/ghbehvbbk.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gynguliqz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gzypdxkbs.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/grqjuwagu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gvzaroger.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gbueukuod.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gsqgubgze.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gvajzxrrs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gefqpslav.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gaqltyfae.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gqmeygukv.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gzhwkwpqu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gxmddmlfv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjmlarnnk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gvfztmevc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqbicowfy.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gmpzcywwf.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gnquytdwe.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/grheedttm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gbqfjpbth.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/ghwegqych.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gqoroycbw.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gkhbjxsni.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/ggfvgtkzg.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/guggqyjst.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/ghfyldzlz.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gndxmwbqh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/ghwpuzblg.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gosfgchxc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gfvaiofwg.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/ggpykgbvc.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gjsisopth.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gfyjshtou.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gvfxfbypu.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gmpruqikt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gepolyfol.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/giskegxwf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gamraubuf.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gpdsxlxtk.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gppdiykpy.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/ggujamxjt.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gleiirkfr.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gwopmoncy.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gacyxmdzu.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/geszcjahz.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gwgihhdds.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/goitjlxfx.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gezvhdthw.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gvirxxlza.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gefzkgqaa.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gttbdefyo.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gmzynzcop.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gpvqbblsr.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gwfpqbmil.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gyvcggwnw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gkswzvbzj.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/grfnwpgyv.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gddogiwhs.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gyvnpqkku.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/ggayjrwxl.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gfxyzpsqi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gslelritc.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gytcycmmt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gjcqyogkz.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gnmzskvqe.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gsvghrtql.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gqhvpbdli.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gzmbuzujs.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gyrdsikrt.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gfsjmrsfh.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gsgqroyzy.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gntuiipqu.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gvxcotkvn.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gdmlelkqz.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gxdequsak.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gonxtowki.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gjmcojzxd.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gwyfkdmjp.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/geywkectb.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gxswaaqqx.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/grizcrvhs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/grzdvdvem.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gsfbltetm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gwjmlhlvc.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gxticcgwv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/geudojazd.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gniqydpom.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gbzblqrbz.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gsdakswpr.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gmiprjbbo.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gvsrcsdmv.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gvwiqxxhs.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/grvfadnos.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gudtdqigp.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gmnmeaxmj.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gkxpxmtpy.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gbiacjuhf.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/ggejlhewa.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gtgnerrso.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gapvlzfxs.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gmnrwytke.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gwszycltg.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/glactlytz.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gjcnxvpyo.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gvoxsloln.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gqbfrrgmv.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gzjmjqdjv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gqeogyuqz.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/ghhnxfols.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gelojnfcw.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gvgenecsc.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/ganpadlpk.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/gzxlrnawl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/ggqljftfa.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gjocefbmi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gdfsebhwb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gcgtcxsmq.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/giagpvrkh.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gxlxbphfn.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gzfukmeej.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gfmsyprik.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gfoxjclqs.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/ggiqqtwbn.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gemoglwwy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/giymwcxfp.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gaxripwen.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gttjbsnsy.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/githqqyjk.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gqjkddmsz.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/geagxeznj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/ginplnqfn.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gjmwsegmz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/ggkrvaarw.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gbbjtapdd.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gfrnglzpy.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gixnumphx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/girezfsbo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggltynsid.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gbacnttqx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gijrgoylt.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gpxdqldjg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/goodbsmcf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gbncpprug.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gwficfzaq.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gvorgijrm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gsufkqzac.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gzgjaanjv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gxenilynx.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gdtnodiod.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gwjuzwvln.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gaobnzhdl.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gsjonjiyx.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gbgyoxemt.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gqmhkzxka.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/givforbby.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gsjkrjvkl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gttopwizl.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gfycalcfv.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gvxdyimjk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gdttgsqgi.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gmswadmhw.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gdnhmzuue.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gmdkpipql.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/ghzzajliz.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gmsqysvex.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gvczlseyo.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gecpizwna.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gapuennnb.sHtML


<!-- 参考信息 -->