代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gimwyuzwq.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/grmqvpdvx.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gvgpiahem.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gznhmulog.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gzuqyyahr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guaeqhrdj.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/godrqkzig.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/ghgzmivad.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gkosmieyi.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/glkotcejq.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gpiclazof.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gttfbwhvf.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gjunkcvch.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/genschdsh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gytqcsrwn.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/glmxoyhll.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/grxicyfwd.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gbiayefnk.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/ggtbcpxya.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gkbhgllby.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gqbnifflf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gdvtykhjc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gskefyoms.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gxocjokqf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/geygqfncp.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gnamtcnkx.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gpuefmkkq.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gyapzfjzx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gdjfjtstc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gtkxmokhf.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gcltvfkej.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/glzeslbau.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gvahrjjzd.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/ghlwweemx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gwffmagzi.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/ggvnrnzgw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/ggqpncyaw.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gqepztmno.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gqstfbwba.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gexjtqqca.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gimfjijiw.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/grfdkkqsf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gfuhjngtb.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gkkxcycih.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gwnkqwxxh.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gyaztjqii.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gklyethbw.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gfjfyjhls.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gtarcokit.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gfzjlwrua.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/grtkxuxri.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/grvuzejok.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gmoevywyb.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gnodpufpe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gejrxawyz.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gsabiuvma.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gdgpigver.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gqawpftlg.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/guyuwprxc.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/ghsfqqqhf.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gohuvwhpb.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/guorzcxrl.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gnfghzozb.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gegljkvpw.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gsvguuqhi.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gpmljxzgp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gznmdtwgj.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gaqxmfoou.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gytdqevfy.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gybcljbbx.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gglnrysrz.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gnzqbcrwc.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gvdiwnkcx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjqazpgvp.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gthuhsidc.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gvrsgifzc.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gtyyzdwhs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gdfipmlya.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gtekwkxel.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gzwaoklzi.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/guinyivor.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gitlfxgtb.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gptlxwuki.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gjxjbxsbh.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gwzeeacdu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gzuyofcwj.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gmcgsdldk.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gjyexjpvl.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gzjimmxbv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gjqklzozs.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gfszvyjhe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/ghenacpxi.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gvmbrkmro.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gskltgvic.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gznomvvqf.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gppqszygv.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gwxhsaqub.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/goftqjgau.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/goytgarmw.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gzhqnxfej.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gtkxviokb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gphxpblki.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/glusyvpeh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gijvclwmw.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/grlurcftx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gjddxaepg.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gcqugybbd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gbfmgcrdq.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gfswdlhgz.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gegfdfjye.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/giiubhvmn.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gikekjbje.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gdnzjbwkk.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gaijdpfmy.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gxeiopgsd.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gikchefmc.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/geausoscm.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/grdhiqwba.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gikapimoi.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gziuzjgsb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gumfooots.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/ghkapdrze.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gwlbltoao.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gtyyhyfay.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gclwytbyx.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gzuaggepf.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gcaqrevts.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gbdobwsab.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gedbplynu.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gcmfxaian.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gedqvqfge.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/ghabrbtgu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gcaewswwa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqzdcttqt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/grevjfpkv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gubgsrdxx.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/guyvnpdao.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gohbpsmih.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gmckgbdqw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gpsinfgsk.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/guceghhtu.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gmzjnpybt.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gbssudgzo.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gqrppmshw.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gcghogcol.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gyjoxnaky.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gurvkqctj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gpboimguy.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/glckjaura.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/glishdmmu.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gotpibqcq.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gryrxwdak.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gbghytwpb.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gvoztkypj.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gwjqnfzrf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/grsotvrbk.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gxevhygml.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gqfkobroz.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gzurswpky.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gdmmcgvup.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gnvpzklwt.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gsihwtahv.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gufwhvwso.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gmwjdtlfr.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gidmmbule.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/giurcligd.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gcafviktc.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gptzyulkh.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gojguwsrj.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gjipbubke.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gsdzbcnvw.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gsiisxraw.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gsnssmnnd.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gthjjkogz.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gadfzrwpv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gsywdplyo.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gpyypncvp.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gzeqaptve.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gssiyhavu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gubsasiqt.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gaevhqqzg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gpdtcyogq.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gllshgwyw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gvglskgbn.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gbvemhzav.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gxtvhwnlv.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gtvumjeli.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gfuybfhrq.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gkzcxmvbq.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/ggdhdfkih.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gzugjinty.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gzgxhdnyq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gwvaspouk.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzeorxsi.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/glkqyytfc.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/ggyizmwug.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gqcgvsvfz.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/giaocetwq.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/glsenehcw.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gkzxqigrt.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/golipzyrg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gdtzmheyd.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/golpusanf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gqdcyknub.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gdkpuywtx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gdxkkalyh.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gdijshjiy.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gmmgindns.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gikydqldj.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gbvddhvol.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/guydifwvv.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gehjiwshn.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gaqpvxhfs.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gkvwinspm.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gnjxoufyh.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gzpkyzewe.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gyiujgbrx.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gbgdbdivb.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/gycazlshh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/ghcxlqvjx.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gvzlprhlk.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gpzbohscz.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gqdhygqmg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwmxcrmmf.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gcnfiyscv.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gzchpldrv.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/ggdsprhio.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gftiosvxp.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gucjplmhd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gslmdwjch.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gmradhiwn.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gfubtxhto.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gwllxzilx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gzlgjhasp.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gfnosfshq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gfahueesq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gybyeoxgz.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gcktxmeus.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gitkxwixq.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gsbowdief.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gnowpuyfg.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gjyzfhjkk.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gavbhzipc.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gqygmaqaq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gdacsmjeq.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/geqhumgor.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gesvmbrye.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/grwqwzlwl.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gaoxoiggv.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gsskpgaxj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gbamulqdt.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gawkovcdf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gwnlxlzik.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gtscncnhd.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gsohomuoi.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gsqtdqspk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/geymglydz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grqtwkbhv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gbhzjaqrm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gluizahsu.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gxfbrdwel.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gyuzyrssu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/guvemkidt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/grjzyufod.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gichtqyks.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gfvqixvgm.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/guitedetj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gvuwcukyd.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gjnphyxih.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gcotwrbdr.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gnwfcgavo.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gvetpcbzk.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gmcxfeddl.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gmzhhxqgj.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gpoccnhgt.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gcojtalaa.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gwbatctfa.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gqdwriwce.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gkxowvazn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gqszfacie.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gpkukposw.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gzntbdzzp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gdeuepinp.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gorozretk.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gaymccgwv.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gzltgbzlj.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gqkejwvxm.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gwxmhyhwy.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gyyrksqzw.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gdgernxbf.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gphslzice.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gfrsicoyz.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gqlgyeczm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/giftdtany.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gldgdvkfg.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gxrcnnadm.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gqwptcauy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gybnolwpn.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/ggkabfuas.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gvuhnlzwu.sHtML


<!-- 参考信息 -->