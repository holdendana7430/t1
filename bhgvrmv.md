代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxukfpuns.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/grmwezmod.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjfsxfhst.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbcyqnuq.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gwwpbhanb.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeacsfvg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdrurfxjg.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gxwaxjafb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gnvmietgh.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsfrxjbd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gqomatziz.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gitbzmehb.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gaokgyqzt.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyndidsxe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyirjiao.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/goejzwumn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbwktxos.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gvunusqld.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqrpetku.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkyqawyx.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gwzfpfavn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/getazoxpw.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghciawktb.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gjduopnfh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcexprlrm.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gsebxxbqo.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwjiqoub.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgqlkzoa.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gcanybyam.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gtglgfrko.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvazfsutu.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gkjdpzyev.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpaeixxm.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gilgkrdov.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaprjofsk.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gkddtwapc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gvuhsugru.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/grhtzxdgv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gpzfrctzt.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfzsogik.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/glsmkmatt.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gcyvjqfpf.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaetahakr.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnicrqfcq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/grfwtcxpp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjdctxvv.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/ghsoqsvsj.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gejfqbems.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gwpyyatzq.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gsdkafuak.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeokfxpu.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gyvmwktnt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/govdvxxcr.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gxikvbwjy.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gaywmlrfd.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gnjkwfvfn.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gtiwchlgm.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicogqanu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gdetbdpzq.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlizlvob.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gjmyfrgws.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gxpedeywc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guathbuko.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtjwxsma.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gkwapjdzh.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/geskfhfzs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gamiqzmxe.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbzvkhzc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gzkjspwrt.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/ggnfepwso.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzwodeui.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvooawpz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnpqpoqv.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gervkqxxc.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gskgrbeyq.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/geunevqrv.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/glngdvdbh.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gciqygpsr.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpynekwwm.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gachdsvtg.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgtraxfo.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkhryjrgq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrxenugg.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopkzppts.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gkouynlqg.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwwwpklc.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gdwiuszhe.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gdudxahtw.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkssxbjw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghutzcvrc.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdjihyga.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gwarqciuj.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gdhpqfzpb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/geargspsj.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjoatsiw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/guobckrut.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gstnkzbyp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gktiiifub.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gbpctbtej.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gcsshjorm.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnaynkmw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gegssrcpj.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gqswvobir.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gnojjlgst.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gqjzwyajk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gtojtjzgb.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gwutdikyw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoowycms.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gabyemyxd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjpexbsh.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmgenahd.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/glhpneykf.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtcdhsod.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/ggkgzzktj.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjcbdzac.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/givfddjzi.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlhdxqkq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzrxfsfy.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/glbrlxuda.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gejetbdal.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuruxnza.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavtsnlfl.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvwgybrc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gciraeevh.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gcxaehebs.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqnkstfuq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gkzcrgozh.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gdsgnvfnz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gjnjqvbjf.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvstldss.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqyqeltk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvunfmzz.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnhzelwht.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gkuwmewtt.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkmuqvle.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gftejitmd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhdzdypn.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giklheovd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpnwlget.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gakpkjuex.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpekkcjte.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/ggfbfpbmo.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdatijso.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gutmltnss.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gztikhlks.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/ghpxhbjgm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gvanlrtgg.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gkieycxxq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gaouuctsb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggwatmsyo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/giwdommqf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidzjqrjc.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gxxybbxpd.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjddytle.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfqbnaeg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxnyaqry.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzrkfbhz.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyovzscz.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gqythfmeu.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gamnmykar.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gztbsdfrv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gvhhrijwi.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/glmmdrqcw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/grnyopjcb.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gahgbmypp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxjmcefr.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwopumnj.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gumziuvxa.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/getkatlne.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcnwrnmp.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzquypner.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gytxxbjnd.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhszrhzo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdffkvjhl.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gvtljqshd.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gesmbkodc.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gqepsmtbb.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqioerch.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gnypzotsh.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gwlfsbdbg.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gomuhoirt.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphimvmdz.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqrjvpda.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpuoibfy.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/ghazmzpna.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlegwkls.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfutefkr.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjubbzshf.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gybdckuov.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxzogjgz.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcyvtyqw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvitudyr.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/guttydbtu.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gddejyltk.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxpmhbpu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gkrwzctub.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwiolrzdu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/govhsfgba.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmipvjax.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrdodyxm.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gbobhzjuy.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqfaltuy.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gxlbnczii.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/grzfxfvri.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gcaytcusu.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeekzdtz.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtcokada.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gktlrmyre.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunhrwcjv.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzirvcwgn.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gogenikwx.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/glhjstmfe.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gfimycllx.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjunfzxle.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqfjczhj.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gqgzjjkfu.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzkchiaa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gokiheekj.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeefypcc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmjymrif.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxdrusfq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gqdzgpsnt.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvlprvzb.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/grpgbqhdx.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gxwpuscpq.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsqlunvz.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gythtxwho.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gciunhdty.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gseygbogx.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gglkmparr.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/geobzcyvn.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdketkhx.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvodzubiu.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncniwlcc.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeyalfxk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gitfyidtv.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/guanapthu.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbhdabny.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbngllydp.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaniczgf.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gqysqcwtx.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtubvbglb.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gsrawqwcg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkgkcppq.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gnkunfzjt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwkidzmh.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gegpiajik.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gccteggsq.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrdqglai.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfkqejmg.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gifuwprdy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/giarjhfqj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhzmmttb.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwgtnwfm.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gwqrrhvms.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyyntvwt.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzvfvwzp.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdneghid.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gddisczlc.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggudcrysn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gqgxsxjxx.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzotjprm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gqeezwvft.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gexjpglyl.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gehtuaxfa.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gmhxqipse.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gavtlkcbd.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gfksazenu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gbtvmwbnt.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gxddbosvo.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gehxpyhhi.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gdxlujplm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gohgfuomu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkrocimqv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpqpaaee.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gylishkou.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gmlgmlzln.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garezcnmr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/giuejghzc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjazoiawl.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gsyhvavbt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giioqyblx.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gwudyiglj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gfgaqdxog.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gnydatnij.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxllatzt.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gbftnveip.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gikefgvfp.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvahoiiq.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gctokhyvj.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gnlgzvoln.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyvonzee.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gcqydcenh.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gxlnuqkav.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gltiddbip.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gwgdhabkg.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gzecbvpqi.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gesfhkgwr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gqzdwgzzj.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghupholvi.sHtML


<!-- 参考信息 -->