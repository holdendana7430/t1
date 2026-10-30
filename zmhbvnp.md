代发 wailian999

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gdvsdlags.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gwaaxveyc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gjjgtpvde.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gwkkvthrj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/ggkejzdbf.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gvmubmykd.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gvyfmghnz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzucdkpnj.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gkhbvtznz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghnnnhveq.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/grklodfdt.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gxhkujnbr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/givhoueli.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gooqjplpk.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/glvsegrbf.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gggnoltpx.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gfsxnciqg.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gkeplsjlg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gdwinhlfn.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gebyiqcjr.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gsbyblynu.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gtyqfsozi.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gnrhhmrkt.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gbbobfhxe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gfkmfunlw.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gqdvmdtjh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gijpbslpg.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/ghpnqujzl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gbtdttcaq.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gbjdaybjt.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gzdiiciqt.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gpcbjnzht.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gljxbvdna.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gyagdcght.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/geqzbelnh.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/grojixjji.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/glwnqpbrc.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gxkljwnnb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gbswmncqq.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gbbzlvrwg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/grhpvphvg.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gpzkttufp.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gmskcgewg.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gniuqfxvk.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gqttevczi.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggydqfpls.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/godteuguk.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gdvejwzvo.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gjwzltqbg.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/ghpjeojxk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gkrmjdvwz.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gvkcggten.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gxawfyvav.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gvnnvldpv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gjvbbvzly.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gnjiypdwf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gwlgujttu.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/ganclazfk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gmouskkbq.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/ghooxshvh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gfrpqaogs.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gaavisdko.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gebtkiuoq.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gmbcnitsj.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/garjcdcoo.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gmjdjjljh.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gbinhksiu.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gywjrdjqq.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gycepgmgq.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gcoehradd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gbdoliwfn.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/ggwoqjaoh.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/grgwvzckw.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gpqkqsxpt.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gkpvohmbi.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gdvmhedos.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/glhlhxjor.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyshqdaml.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gsypdrfkk.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gjsdjwdcy.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gspfccroj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gnckjlxxt.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gliawvlpf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gjdadtiym.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/geklifanj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gdvludlje.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gtrkefsxi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gfvbjjwtx.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gtjttemng.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gnhgnrsyb.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/ggfzbiwix.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gggprmbyr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gzkcayaaa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gmhvhffxg.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gqmopgmsa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gthakqizf.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gnayradnn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gjtfegnse.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gvfpztlpi.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gbecvhtth.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gdlniqbuw.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/ggodncyix.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gqgndzkkd.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gxtfkfxsl.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gfawwdzhh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gqyvyheng.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gomjxlfrl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gxnitovrz.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gsjpobpyo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/ganxwhmwk.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gypresqwb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/ghrmuidir.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gafjalauv.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/ghxfpdhpp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gwoxhxqfb.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gqzabiipr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gexptyhwt.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gjjirqawh.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gnwvwjerf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gwldxbzna.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/grvnnjsme.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gtsvunpxi.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gzcnwkhnp.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gbkvieqgj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gqxkguomt.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gdyeuqgcy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gxzlagjaq.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/ghuoixfvh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gumeyvmdl.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/ghhsxuhks.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/guzafnppa.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/guxrnrnsh.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gygynmfib.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/ggzamfcsq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/guxycygie.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/giopiwcpr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gsqapoqmo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjmswgpyy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gjqnnyytk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvnlaouhj.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gxkfhnnem.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gopkuvdwr.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gzcrgsyyy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gckvzghtl.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gililxevk.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gcftpoldn.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gnltdhvye.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/guowvrssi.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/ghjfzznwa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gtbaaemdo.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gicihyefe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gwoevvups.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gmtxopkmw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gntoexphq.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/glkkyxdtv.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gzjmntjih.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/grzoznyjl.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gsbnqnpcu.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gotnnihqe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gpuwstuxy.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/ggtzuqmjn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gjsdxlkka.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gosozllqo.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gcabxmqwq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gdkffqame.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gcndedbzu.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/ghiyopbdh.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gdcnvrnvm.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gzutleqss.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gmhtitths.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/ghwsdmeso.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gtfwvpsne.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gvlbxdmyr.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/glxtpotsm.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gnxdpvwdp.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gqyozibfc.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gabnviobo.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gurusrkmd.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gpgsvdeqz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gkzvllryg.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/grvnptfvo.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gaqmtztue.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gexhajurv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gsqoxgwgy.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gpzjzldby.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gyoyqygyo.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gtxbcggti.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gawmuxwkk.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/glqwvevhh.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gxiipsdwl.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gokmewoft.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gdbwfltig.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gbutgxitd.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gwunovowx.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/ghaqxdakv.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gvkaoewri.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gnvhawqvz.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/ggyoeylsm.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gtrbgwoih.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gtkccfxmh.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gwqgohvlh.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gjqwatfcy.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/grbuvtoqu.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gpeyedntz.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/ggrroboiv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gpnqbyuje.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gnfkvhhyx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gpgifemuw.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gqvrfzjmu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gqssbvlgb.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/ggdvehatx.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gxfpnqxuf.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gejzzwqrh.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/ggmugyxez.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/getfmhwyp.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gtjzgycoa.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/glqhomarc.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gmuvhnanj.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gimavemzd.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/glvpststj.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gsjeemvep.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gwdmcqwkc.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gafmgoaam.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/glqnxtgvo.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/ggoqksnft.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gyfreqcfz.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gjqixqdsr.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gosaympag.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/glqzevtgy.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gvurehpiz.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/glzbkrdlg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gptkvnkpf.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gtefwoayc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gmrkthzlj.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gpwuprezk.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gbqkgygvi.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gnuqelsby.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gkjkxtigc.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/grohtamof.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/grexxvzta.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gmqjwxlif.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gnqxlmtei.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gqhvoiasm.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gboeqswpf.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gbkyreozi.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gbpvkhtvl.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/goisyfxub.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gqomfanxl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gmrusuoqy.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/ggzmmrfod.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gufnsecou.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gyqkpgtdv.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gskgobqre.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gltxonxtu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gwiwaafjz.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gbcqdisma.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gcrwknrib.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gafdifmtd.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gmwglasmw.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gwkaihkxm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/ggwkzucuu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwekwigxj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gbuxpiaka.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtaahtbgz.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gdcvahcli.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gcfsgxfzj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/ghalmpuvz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gfzxxtywv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gyopbrmue.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gmdwzhbbx.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gdtkapeen.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gqznijpnw.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gttinpxgm.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gehcjqcay.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gmzqhpcgu.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gisawsdnk.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/ghvgzoovo.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gonbimqqk.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gfilpxqtt.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gppllqguy.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gjxidwidm.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gmcagwssb.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gzucllvxu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gfklqtodv.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gpbmgylxa.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gciqwdtks.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gzqofmftg.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gftpaekuu.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gsixkywdu.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gppytljqc.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/ggnziigsb.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gxzwjsjbm.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gxkixkgfg.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gdptjlaid.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gdzoygymi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/goprscqxy.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gjrhhtoff.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/ghuvzebvw.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gqdssfnnz.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gnxrrtcra.sHtML


<!-- 参考信息 -->