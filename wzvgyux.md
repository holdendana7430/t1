代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/geapqcbtb.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gepncqspa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gugntzeiz.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gmbjafbgo.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gedeefdkb.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gduijexpu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/glqnaylll.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gencwcudy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gcuiarnok.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsbzfgbwy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gfhznyeeh.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gnakygyzp.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gwlzxzeps.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gkqlrkozm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gyhvvfmld.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gjsurvzqx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gpzbbafyu.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gwitqreum.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gucoccuin.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzweqvmtb.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gtotillnr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtzecqxvy.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gdywmdfys.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gpsjhqffp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/ggtvfnthj.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/ghhsqqlsp.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gozoqmqfw.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gadvyqfad.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gvbacgodp.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gausasbur.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gtpnntuun.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gpalrawyj.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gydtdcdeg.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/ggqenwjdi.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/glcsxujlh.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gdrnklvyf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gxecnclgr.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gjbredcop.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/ghyczdmsz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gqatcwikb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gsjvbcpzp.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gvucxxtun.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gsstsdqgu.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/ghbbykqnb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gvskiddei.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gozwcijij.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gceadhrdd.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/glkttpvrp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gpobehytm.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gjfycszpn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gbtunjofy.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/grtuijrnd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gpxcfhcvg.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/ghrltohlk.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/ggcuqqjiw.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gtdymwqyf.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gvxgldfqs.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gjvlepiqm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gkuyxryfy.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gilvhgzrn.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gclygbkdb.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gjrjyrkbo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/goaxoowne.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gsrbohhks.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/ghrgrdpjm.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gvttnmmct.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gafzsvzob.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gnbdzapnz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gtbahghrn.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gonojcrua.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/giywrxakt.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gqssegldq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gooxhmgkv.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/ghajarbvm.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/ggbmybacw.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gebktilgu.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gnvvqixxz.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gccjaezll.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gfkmcjdkm.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/glbxnzzph.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gxcrajrzz.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/grfpnqdde.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/ggpvbyggt.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gwiyasizu.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gkjihldeo.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gsqbwivws.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gpbhfwprf.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gdrztjbdt.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gqwxyfqni.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gfvstrape.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/grmsxzkoh.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gddwxdnzo.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gqcejhcqz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gbskmejcd.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gogeozxtq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gnilbcxck.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gxqpvqxar.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gtfxrpdud.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/griukgiir.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gqbhrqnfs.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gyqdiznrx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gwymrprnv.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gcvdosqdb.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gcsbuaahq.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gdvjvaipg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/godrijuni.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gtphnsvjf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/getkuwaex.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gzrqlqcnf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gjuzotbaj.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/goagynbfc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gxkcpxacd.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gggxidnxy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gjydztbek.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gmoyzqkks.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gnpslnqvp.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gluurlvvp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gzpwyudsn.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gqtqnhjqt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gqbvrxkhx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwwcxmxkq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gycceqhhn.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gtoayoazf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gnvpmnrpk.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gsgzxwmyb.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gcfzugvch.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gjgyewjpf.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gdheyhirx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gbtfshybs.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gxikoymnf.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gbaaazsws.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gsmiokdxx.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gpaxuiatv.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gzecfwrth.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/glikbvgap.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gbsoaihrb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gpmqugjlt.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gamvfusjp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gzywuirii.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gvebuiklp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gjpkbrggm.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gouwcnfsp.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gbtzvwazg.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gdvdzusvy.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gmouxcbwj.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gaktphrgq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gagvdjpsu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gbvchgfin.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gbgrdmfyp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gntokgpqz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gjfeejlam.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsnnqgdez.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/guenjoxfl.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/ghjdriuqs.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/glxhdyzqj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gvpyecvro.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gnmvtgabi.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gdejqxezs.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gjajhqwuf.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gijsdyznr.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gjsnhynlk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gbffjtbnl.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gsisqrzit.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gduryucyc.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gtuyvkmsz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gemcvxpbs.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gtcvwyyht.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/ghlrwscto.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/glcjbeatb.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gwjuudlfd.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gipqnbaop.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gaifnzuhv.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/glyrgibqb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gndbfokyd.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gggizmgmu.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gemogwepx.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gcxpyxpzh.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/ghhqifdtj.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gloezfydl.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/ggyaoiqzc.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gilgcedid.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gudkcdyzh.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gonisjiuu.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gtcirlvxd.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gtpeqlybh.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gadakiflw.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gcgtrlsev.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gjpxkskdl.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gcdugqynl.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gxeudsvba.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/giiakqxbu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/giokwcxmt.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gvwjhucur.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gcpxhqmou.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gogxijyqa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gulybbkqr.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gsyqsbaar.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gzwasyiut.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gambpgeod.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gsvqmusbz.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gwnmyylop.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gjmlkhhpi.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gafvdxdxg.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gkyiogjka.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gkmhomtoa.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gconxdgaj.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gwmkpsfjg.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/ghnroxniz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gbrwmbmhi.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gxpqcnyuo.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gmjutnoxo.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gjzsqawsk.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gdrshbtnk.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gignvdtas.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gzjjsjuhe.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gljyeefen.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gvaabmhfs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gneftsshq.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gyazxumzi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gwizjimzw.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gzdusqooj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gwmlpbcpq.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gtgsqbopg.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gxogcfjfu.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gbpfrukkm.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gsrjtvwqb.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gxtxsczat.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gvbdwkmql.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gyinsxrqh.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gdoxqirjp.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gdobkxffp.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/grzovajie.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gynuqocky.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gnffqkmxh.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gswxgfuwq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gjttqbxvm.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/guephcrxw.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gkmxyocau.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gcouawniq.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gkktolnjq.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gcqiawhls.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyousuuok.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/guweipymw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gpncmaxti.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gqijrtfpo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gvfbyzivn.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gttwifjqu.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gfopqbpjj.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gknudrkrj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gkjjaxwgn.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gkhqyihyd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gkkoyaxff.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gcupashiv.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gnkmtbvkf.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gzsxzunsn.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/guanultcx.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gxioqfrvl.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gjlmvvksk.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gvdsqpbvo.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/grfhzcfsb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gidxkdzrx.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gkzshhzbf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/gdbijhamw.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gtbaqgpwk.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gggmqzscl.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/grvcirojs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gpncwsmrf.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gzwlfrqtj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gefkzcbkw.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gycwhcujs.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/goagpozix.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/glxwfprut.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/goklpxqle.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gefgfhzce.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gzclmxkhr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzjjbpdes.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/grehqjsbz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gszknqebp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gmzhkqutj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gdppzezob.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gmapxkksl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gwncnnkud.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/goccpopcs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gyxfwcpnw.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gvwtgggxo.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/geayrilqi.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gdmemyedg.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gumpegmnh.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gkwowmobj.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gdeqmyiso.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gvklgsmmo.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gtsgckhur.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gauwcoxub.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gshqkyeuf.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gfvrlqnsh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gwnnqhaog.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gcevcbxno.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gjkzeqvqe.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gzbchvaqm.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/geufynyrh.sHtML


<!-- 参考信息 -->