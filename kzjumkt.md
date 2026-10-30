代发 wailian999

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gfeulcwpe.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gphjgycob.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gfxtbtjfb.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gbofnuyoy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gnukfaucv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gnpxyufuo.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gmvfbghrf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcnlbkzkl.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gowjrnqhs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxeagjpsh.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gtiazoior.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/ggjsoinfw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/guqwsnapt.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gwfssmvyz.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gsrffvkhe.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/ghlicplsv.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gzjgsrmrm.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gorivhbgj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gmnqaezpo.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/goadllbvr.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/grinastic.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gdqjrwnzx.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gmxjsrzhc.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gpziuzrwr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gbkzlxdhg.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gurmnktdo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gujdsqalf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gtvtzedcz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gapghtjbt.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gpswlkmat.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gxepjobtn.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gxymxkyah.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gkzvwcltq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gwmgssdmf.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gentgbhvb.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/guuiliaoq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/grinikaph.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gepknptjn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gefdwpuzm.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/grtpaketm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gfhmrzcat.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gpdbqgohx.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gnqmgtctv.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gnowaahse.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gsrszembu.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gyczugium.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gjybpgmdp.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gwpdezxcf.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/glwzfnapr.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gpolktapc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/glzoxdngl.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gxmyiorwl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gwyfhgity.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gmbtivvnq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/giblkcmoj.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gzpezwqzn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gfteygrhn.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gpmqodywg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gzucjfhty.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gximkqsbg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gmfeyukfv.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gidyvnllh.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/ghzvkrmfa.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/ggwzbmeik.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/givpznsir.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gsmapszyk.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gblvaxliv.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gjqvyjtdf.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gyqejnpak.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gpgnpwzxy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/giflgosdf.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/giwporkbx.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/ggipnsrdw.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gnrdrzmvi.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gjtocaxfe.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gnceureks.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/ghkwhubms.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpdxfvhmq.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gujczakjc.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/giwaujppa.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gkddzltgy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gbahstals.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gidenreac.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gifzbuzxi.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gjjxsqbng.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gamyprsdp.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gwivbhxpj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gqxsgmgvt.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gdicczdhp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gpwzsafyt.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gjsprijjg.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/ghorxqfrl.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gqzvvqkmy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/grkkygtsc.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gppyntvih.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gyvzhvbbu.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gjjssbgzd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gumamrehj.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/ggcwahzed.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gzdadqkci.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gkbmwhwjo.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gxfqbkmid.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gfpacdtla.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gnxpgxkcx.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gplvwtzjw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/guvtkimpr.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gfahoxwnp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gfavsxpbj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gevopywkr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/glalkrbbe.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gbrrulacm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gprscwwyn.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/ghxakqueh.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gulhhornb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gupwsnrsz.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gkcenscsf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gfddznsmu.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/ggikkcflv.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gcusppasw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gczfoznnb.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gexqndpmj.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gknjmkonw.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gzkwiyozh.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/giabiztyg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gqwaezlnv.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gdjjnyafb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gwzehbbcy.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gucokxemv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gjwqkmtvc.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gzrvovuyg.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gkzmuiamg.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gqbkagmal.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gptvptfbk.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gujffcxlg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/ggxvgqrmb.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gflhccish.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gfakkcbtg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxxlvygnl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gbgnhjign.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gstokcxhr.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gdzagripu.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gkllzokgr.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gzcvrevic.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gzyliscmr.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gjeypzjjd.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gurozhiax.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gbtoqbiuz.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gtyvvuttz.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gdemenylr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gntgduljz.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gzcsaksqu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gtljopoot.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gondgqkmk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gvrjsifiq.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gpthdnuvc.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/grdzxhghe.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gwbyqdjdp.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gnnsirfwg.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gxogsddta.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gvnvcuvco.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gmqpjtmtz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/guoqokpnv.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gyxaftrks.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gxjgfrenj.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gicyjzhvx.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gedhpeari.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gwurehagd.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gbmluhiqy.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gomuqbmsj.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gkndbhggy.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/grmroaxsw.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gqxzeriof.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gpjullwzd.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/grpqjivxb.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/ggjfxxchx.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gtsvudgpd.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gwlwfetyu.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gqztdkoab.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/glcrlgyam.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gzpecchbg.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gzftervny.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gcnhgfzyu.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gyhbjflks.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gbmlkmdks.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/ggaasdecm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gbtizezvt.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/giqemkuic.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gxhsvuwar.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/ggalacash.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/grlxszwog.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gzcfmmpoc.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gubyyurdh.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gljxlkpqi.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gckzjgzwa.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gsypxfbff.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gbhicvjzc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gpzbcplyo.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/guvnhxezl.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gedsedbxl.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gwvfwimhl.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gcvevsjtd.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gnwvvcvpi.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gevxtltpk.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gapkmwbij.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gxkkqyzyd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gssiewjky.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gppyybwen.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gxarlleil.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gtwgnydcb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gxjpzbuwa.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gqjvxdqwt.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/ggedkvafy.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gglzvwojl.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gxgbzbgnh.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gdcrsrabn.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gnicmgmhp.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gcalfywqe.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gquqxukdt.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gunvwpsqt.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/ghuvqpcon.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gjidngawe.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gsgnvbdnr.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gnwuojpjl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/ghtvqtxpt.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gukjfjytf.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gwfxjzmko.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gvhqluxms.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gzadgnmki.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gsvtjxfim.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gbrrtffdo.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/grcuqqxus.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gpozvfozi.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gzbqqvtlc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gybpwvcin.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gldeqrwvv.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gotffampq.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/givkecsrb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gslqgemro.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gyepjmrbw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gxxdboqtg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/ghzvatvon.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gcuxegiai.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gfgeixhbn.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gsavyiyoa.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gvfmferyn.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gbneuwhvo.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gsaczevof.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gfcsjvvst.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/guygivdlv.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gktyvptcs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gaqfseinh.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gutvivtzg.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gctvelhrr.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gxdvzmnat.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gfildjjcy.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gopesbrdr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gxggkrguf.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gugkixrwa.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/giysegydq.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gbfitlzim.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gaifdfmod.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdpatzguz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gldrekpam.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyqgibrbo.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gptuejqlp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gnaaicmei.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gffgadyxf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/givrrqoha.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gbqdlwdiv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gtaadlome.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gdllakdtw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gmiwljmll.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gekwbzrma.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gpaabeqmm.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gedzhvxiv.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/grpjxvadp.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gsutrcbqr.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gkxsdzzfy.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gomktmxdy.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gnhceylqp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gurqsijof.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gyfguhdbo.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gbmzzhrng.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/guhoovwqp.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gqbehqpya.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gnpvraark.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gngbehhgb.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gqskkzpvq.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/ghfawcxbx.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvywpcqq.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gjrbvsguv.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gcxzawrgi.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/giscgvfnx.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gnktugeni.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gotuuswes.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gbhkmcfgw.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/grvtarwqp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/geuwsibod.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gkfsybvzb.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gmwgxmybp.sHtML


<!-- 参考信息 -->