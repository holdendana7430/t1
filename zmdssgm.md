代发 wailian999

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gmjndkavz.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyylvbmio.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqamtslw.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gqdxfaqzp.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giicbgzul.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtdvulbn.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gwicwqpok.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjmcxczg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjhkrukl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtxvrihi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/ghdflalvv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/geubghsup.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gfypntoyf.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtelcbljf.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxooznjn.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gehxjtzwq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmqlkfsj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqufxbyyz.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcitmthxh.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/glialdlxq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnbffvtc.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/geulwacne.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gllnllljn.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gtijqrdxf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gtouazwbc.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwprarii.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gbaxftzdg.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqarcbyx.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gvoqozmtg.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmjeejzr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/grpnjigxs.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guisrucau.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gxketcsdu.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzrjuyfi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gskvplsbt.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyyvybkv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gjzwndfve.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gxubidpol.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqylpaci.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gaifziqqe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gqphzytuc.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gnwydnlmv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gupiidkes.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gwstawnfj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpecjefsl.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjfqgpbc.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/grzctnaet.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gibynlbno.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqslcqpm.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gbirjvjjo.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxwuwwyq.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnadsfgks.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gkncpabxm.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/grtizuqpc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/geeqmqzbj.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/geglvzrmt.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyllqadf.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/ggrftoyhx.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqllwwepq.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gmsvyatqr.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqawqlya.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwrlsqtfk.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeuwrmnt.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvfxbucf.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqtbmxez.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gezslxfpf.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gtcxzmnue.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gycxwodng.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gjdfhmges.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gynzsbbqo.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/ggsdxnqmh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpiqudgh.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gkjibeizu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrovaxkc.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gokpvofzx.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gnmycroft.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjzcptvh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gmczbdsgs.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gcieqfyhp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghanemtuw.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdguqbhj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeseaips.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/geytdfcmr.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gjhqplrpb.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxrwnhrz.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/goivhgpbh.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gfycledhs.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gimjuxwhg.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhnjmyym.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyoicgup.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/glhkzfgpg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxkmrqtdu.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gqikmdtlb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gangucnui.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfxtnfoww.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfibiius.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxkmkvsv.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzqbawtbn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gmgucgnkd.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjhxorrn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrtueqhy.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gogjvboef.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdwwimnh.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhorqrvd.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbonwufuk.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbacnmwy.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gfnczqhak.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gbsopqgos.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gdfsehrqb.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmakdvvma.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gcgvedhye.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkkafdyb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdejnnkhn.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gajhhuanm.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomlmnuuf.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqhonkks.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwxdmjnx.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwspglfd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gmokfjoku.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gceutpypt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gasdyvggw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gfajrektp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzxsxvym.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gohoduvgb.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gbylexeav.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbogwfkdr.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhkoxuzh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwhlzaxa.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnquvnks.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/guheqoazr.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/glfikeyim.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gongkaggy.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gznrewpyp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gmumwncrt.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gulxiowaq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjpzvnam.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gwiprpelc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggykowxyf.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gpylplpuk.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtajxagqu.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzxsnpfhp.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gffhukbhs.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gkttffyfc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrzvcftc.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemvjqfbd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzctaxehf.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gnommfcye.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzfjljll.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gwqjditfb.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjqoyzvy.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gxqifupjp.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gzdywcryn.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gamshbcns.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/grnvbjwkn.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gmruywfnl.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gednnqhqb.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdsjnicu.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/grntkvnii.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gbpdazjol.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gzvifhqjo.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gcngoqdwd.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gfcbqhlcw.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gdozoqkqw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmakhmag.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gewyfbeyb.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gvgtmofvo.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnymqbgn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjbwumkc.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gumuzaeql.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkxsgrng.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrodxcrs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghumfauod.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gnjjjlgop.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvhfwtaf.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmbtuknk.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjxsyodx.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/grhaammzr.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcufoqfbu.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/guintdchz.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gouvmxill.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/goztqckmr.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkkewlxk.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzegveih.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeucwicc.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gawustzzc.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyidgcso.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgtrggam.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gofwcmnfu.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gawzqolsq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbjbnjsf.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gprwznvlc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gkayihihp.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gidafofix.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/grixvikao.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/glkaiinnl.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grchghuqs.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gdwxdclog.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gwmchdkeg.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gwxzaxalz.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbqeptub.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gacczykxz.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcgczfpw.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gidzqkwmo.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gsecntxaf.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gphroroun.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gtoixyoxo.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gbvrexupu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gswubwmlp.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/giiniffpr.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccembyoc.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gszyxhmse.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwojcncl.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/guobgdbqn.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwunejesn.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/guvaaqtly.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghxjyitzb.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gyceunxgg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqmsvqxwc.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/getpuqglo.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuxmtltp.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhlmeyrh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gexhoywkm.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvwpbvha.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gglyuatay.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlwupoml.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gzyluamcc.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gosnzmoun.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gzujwweld.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhfolaxm.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/grhkdwhqp.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgktredc.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqrexvwy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiruusmo.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gyomfmaro.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/glgcyhroy.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gzioxppzl.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghavyofio.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gkevntmlw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkilclhw.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwczderdl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjxkumwf.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gfyvffzmk.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmrymkdh.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gdlayfjce.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gffrilhbe.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwjzhmte.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gffalegvr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjfhnbqm.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gqfpvuyry.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gohnpyxua.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/getrwejej.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnzdnjqw.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gukqghoqx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpvndwkh.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gamlfbuyb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdfqvuix.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/ghrbdgazj.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gltgmlvlp.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gtxgaqvlr.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcltjnlp.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gnnxehhgn.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmoakidl.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gmjtiyfcb.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gdsdzzjzu.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gwlbsqslc.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoxtmyru.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcebjzzp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzofrboqa.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gmoorguek.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/guevzuaky.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gnntkiimp.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gxladfwyc.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjhstiwc.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/ggmsnusux.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/grqnptiwc.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtjtonpv.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gwkzsjyax.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gogxqgkmr.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/ghshxybrf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gidiuvfed.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gvwwqtjna.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwogubqt.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbveivuk.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexczngaw.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gphlckspo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gchzaeppe.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaxgbchs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gjvhowedh.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdqtkqka.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffcvrozs.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfosxfvp.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggteknzbd.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldzfdbrh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gozcwqwpq.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gclhsvxvi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdnkmwbo.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gnnunqvnl.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gylxywizr.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gjlzrjtjw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gvoimoiyr.sHtML


<!-- 参考信息 -->