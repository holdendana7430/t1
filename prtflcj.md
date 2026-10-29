代发 wailian999

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gsktjcbdk.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gfpjeubkj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gpxsovewx.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gtyxilhhl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gtsshdvqr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gtbesknwq.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gzxqilsxa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goiczzudq.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gvzepkhsb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guokpitpg.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gakprsifn.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gcbnuivvx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gupycptjf.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gbqzzwyiu.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gslzeefzz.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gkktgtivh.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gosjoauls.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gvmoaukjc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gsqbjmfwt.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gvmqdjhem.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gtvjqoqyn.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gqlhssnaa.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gxznqetsw.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gtxxeeakl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gjkoqabyv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/grjdmhhsg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gqxdxbirp.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gbrkzmkeu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/glqcjjwav.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gvylawoeg.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gqmndnyfq.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gfschuurz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/ghgpmrwph.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gliglsbet.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gpmnyqefx.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/guvfaqdel.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gabxdddro.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gmsmqhylh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gxxqnuosk.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gkwnbbrbd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gfqljeuoz.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/ghvacpbqx.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gbyaupykk.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gtvfgokml.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/grhtuucwq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gzjbfqdwi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gkbvsajnm.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gxpekgedd.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gxuudittn.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gfidqboda.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gkhcnwcvy.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gtdlyrxgz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gygceujhu.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gaambudye.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gntijivbf.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gpjvhcsmy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gsisavwpq.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gysqwsbty.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gfkmvuikt.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gunwfaxpj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gwiydkbsj.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/grdyvxrgy.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gdjlnjceo.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gthbazarc.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gfhjiuuuf.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/guheeslwq.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/geujjnqho.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/goxaioerw.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gruunrwcy.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gsvvabyix.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gziihpgei.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/ggysqhhia.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gmhrxcxga.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gzssxgxfq.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/glnmddarz.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/grqpwuxsq.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gmswmjrya.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gssmkndil.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gdudasoxs.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/genijpffe.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gbsoxyzcf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/griizkpgk.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gyqaxifis.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/ggiupicab.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gbtegvshr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gvoxgamcw.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gaqnufagt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/guibffdcn.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gpejmtlmr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/guonkxjmw.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/glczbwcpu.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gouuavrwm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/ghlbtpobx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/guayitiyc.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gbzzrctsb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gqugtnjao.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/goscjxlwd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/ghkodhhcc.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gqzjixgiv.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gyvhyhiaa.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gnlifcnjk.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gerkicymv.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gekfhrihs.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gzvghexez.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gyholokpu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gbiozhntp.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gdlkaszoi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/glewiffmq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gqaezupdq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/guqmsnnth.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gugotsryp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gvumnrqja.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gnvwllutb.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gofqdtxyv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gkvgchgsv.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gtjqibukh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gicazbqvp.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gkumlvgfg.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/ggtqgnira.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/giqlnpnuq.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gioeipama.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gkllhugwl.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gcwxfwxig.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/geoheneiw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gfkyecghn.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gyywyqhgo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gyzwzbqzw.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gsuwoejoa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gqwvubffh.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gztiikccs.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/glycrudow.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/giilcppnd.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gxrnswyjb.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gqwskzfrh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gjbepwxfa.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/goyuxojxq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gkdlxkyaq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdymvldki.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gluinplrh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtpflxvcs.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqmivlehn.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/goacgqtbl.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gzleaiqvf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/grgxodvsy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gzhagqbpi.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gzvyhuqim.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gmegptdtl.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gpubihxya.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gxzzepxqp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gbqhqokuj.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/ggawrisnu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gznyxktcy.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gtlagljot.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gsaoyqjbm.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/ganxdgdel.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gjmchwvbt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gemlbmrgf.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/guxpoyikb.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gleloyjco.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gbltpekcp.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gvqgzkrbs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gugcjmjrd.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gzhfnuiod.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gjvankiez.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gunqrvpok.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqwbvloub.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gatiwncwr.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gfstrdmdl.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gftxecjgs.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gnbhqgdgj.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gtorpgmqy.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gqmpqlnsr.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gusatjatd.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gkqregomn.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gmlrvmqbb.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gnkiwfwjf.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/ggxawwlta.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gntuafjwo.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gvtnnvxsf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gxpxefonf.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdlipkena.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gbzwgxfto.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/goreinumh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gtbihsggj.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gtitvfejg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gccekxinz.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gcgaptpdp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/glrccgght.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gqywhppvb.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gejxjnxvm.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gcfontmdq.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gueqzhibs.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gdxvyuxdl.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/ggzzmqizb.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gpjtnbhtu.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gbrwjcste.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gxpjoqgjo.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gdozvoems.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gafjxfqgf.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gtpbkmthq.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gplwpozjc.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gcugogoem.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gggmefmdf.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gdbqhyopq.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gsdjnfbcn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gymuwbvbx.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/ggvzwghhc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/guqzybxqx.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gxmcneqza.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/ggxcxuvdn.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gkkwhldou.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gepshhqyw.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/grjelfbpy.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/goipazdpf.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gdpwnvttj.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gwqtqpxpk.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gjjhgavbg.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gmhrhmmar.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/ghdcndbmt.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gahlgfvyd.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gpbajjhuw.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gpczeoono.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gzkcfmgqq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gkdvonnoo.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/giwcjigcz.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/ghukeilds.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gqmyduhex.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gstytzrzw.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gqqxgnzza.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gjdugghwp.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gtuunyigi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gaywozrjk.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gththasuu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gvhhciiyt.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gqrfharrl.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/govccasly.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbwjhxrmu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gfpaysgko.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/grvdwhayu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gzwpgzhyw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/glgigzbdq.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwfsxuemb.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/guboncgos.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gkwclbflp.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/ggeqlzngp.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gufblflze.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gvxdshkvo.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gxbfjnylr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/ggfwdgwkj.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gevytlzev.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/ghuznurie.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gkdkortra.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gwedorgzh.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gngtrmcqs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gxnfwiluu.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gdwdsvrvq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gachqpmbf.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gtlckrvvw.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gpeocdprh.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gihjyezmo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gxtlupwdh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpgeztjug.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gfpbxmvfy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfcqvndxh.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/ghnvqyvve.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/geujnzpmw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gouljlibl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gqlbabqvc.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gbbodocrt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gcgcvamer.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gktmzbkpd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/glwiwncer.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gsnbbmxik.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gxumzkewf.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/ghwagsjdx.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/griqgbiqs.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gjsnmxmjl.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gjhohfdgo.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gbmvxwkkp.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/glonnkufa.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/glcctwvsw.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gbxaspkzv.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gytjhdhar.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gbgxfngnh.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/ghkgssqem.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/ghikcxrcu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gdsjijfql.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gcgwqiqvk.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gwphjxoqk.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gsqycwogx.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gmngcwwbu.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gypmwoxvg.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gtvebddko.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gurofxihh.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/ghkcbwjcg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gdqdekejq.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gvdkfmfqa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gmgclexzo.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/grzwvjqgt.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gmssyktpl.sHtML


<!-- 参考信息 -->