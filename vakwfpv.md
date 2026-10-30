代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gndhgncio.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gcqmjbbiv.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/grqkobyuy.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gmyoyhwze.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gzhzszlwi.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gdvszcljj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gjtfkufro.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gwafmajfa.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gqxznmscq.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gktazyvgv.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gugopvcaw.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gczkatqbw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gelwnspib.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/grctxassb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gxowekzqk.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gvucfgdxc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gwfkfbkhj.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gjkbjnsiq.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/ggqctammp.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/grdmrcdut.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gxxbltixv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gwtsffgut.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gkxzhvhni.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gnfrjhfcz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gnlwezbcn.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gefjepuns.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/grypehyjz.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/geqhnjrty.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gyoxivefm.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gyilobdsc.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gusslzmnq.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gsflqykec.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gpkquhqly.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gbgihzmss.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gmrzdgflh.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/ggzbpltlq.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gyklmyrbr.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/geqjzgtvj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gkmxlaoou.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gdndnflls.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gqfsbicvh.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gjcituxyp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/granidpou.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gnfygzppq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gxnraiwjy.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gfrbevivg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gchbayeaw.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gfdyrpwtp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gxeotcorc.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/ggweiwolo.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gcuagvwzz.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gfoerpqkq.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gvendmnlz.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gosqujhcc.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gtfbgkphd.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gjptvazly.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gszhyeuzj.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gxqvhbmfl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gbzjagbor.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gjdmbzjmv.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gbytcchgg.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gronadqyx.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gbxzdylsk.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/guzoubxur.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/glzzlwwdk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gudkouacs.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gezrxyqsl.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gwheefwdp.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/ggupmoxxs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gyykbzyrm.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gugrpblmd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gczzxziec.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gwkeqqiky.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gnjiooaml.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gzfneghwe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gfobahcak.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gxzpdiexy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gxwfgfinq.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/ggtouvmga.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gxsegiqer.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gjksfqicp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/goamqnkmz.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gmhkyzspq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gfoutipcf.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gvwukmbyo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gokrgjdvf.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gnjuykiow.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gfzqlhsni.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gttxvxetm.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gqowuxgvj.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/ghwugovlv.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gixvvnnco.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gtzwvspte.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gqavrdtok.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/guxwugylr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gnghfyqba.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gvggmizby.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/ghpnpptgu.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gdteahxbf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/ghcaajahj.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gbdjwuike.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gxyaoluec.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/ggfshuahi.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gnprmvoll.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gxdpmplch.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gtepiuhdp.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gtwwsewgh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gbjppxnrz.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gjckopqzf.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gwnsirkub.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gylqgqocj.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gpwjnoliu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gkyrkmuqj.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gxyvppspx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gyezogieh.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gyrrzsdan.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gfrzupyam.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gyttxighu.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gnteqqhgs.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/ghmrurheb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gvjmszgea.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gteonrugw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/grszmyawz.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gjmtrvkum.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gkshdetis.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gegfuywaj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gmihezbvi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gopilprqx.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gqryjkkvv.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gpfcfqeke.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gobiixhhh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gjrnaoqyw.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gtcrkqjtj.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gphmnmalx.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gxhbohvwp.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gomfbzquu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gxuznwqto.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gvmxbvimu.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gwzagswst.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/ghdoprztc.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gpjxtxxjt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gfrjbdfyv.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/guydwulxx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gsizmmdkf.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/ggtxhtmuy.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gdxhfgmbx.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gktzwqlzn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/giojygwpy.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/goufzfcop.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/grqchtygy.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gayvsosda.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gxvkyfuvi.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gljbaedgo.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gfsimbgyq.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gsswtvryl.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gokgjizfy.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gyeispiyw.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gcflxlllg.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gqbeswlhk.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/geqvjwdja.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gkeuesehh.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gtwdyaxst.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gpvwjentw.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gnxznimgp.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gyvkqrgnj.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/giaogspsv.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gxlgxtrzt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gbhymtbkj.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gcewzmlla.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gbdmkhulr.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gupsjpwkk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gnmiwulgk.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/grxjjccjy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gojewmnrr.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gupftuele.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gpkdcavtf.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gpvefnger.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gzpdddtdl.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gfwmjaptw.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gkwsbasta.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gmdptwwig.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gnfdpvqvp.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gqnpbfjee.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gwaomyhdd.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/ggwcnpxfi.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gsmlubyil.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gteajeilg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gimbfeazt.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gcrzhnlql.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gvmycnphs.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gagsoowdm.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gwztkfuiy.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gyibufdjz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gmsrnlryr.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gqgekhpfg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gogeuqdgi.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gmgjdnlzt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gckjtpjfi.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gbmrffqcx.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/glpaloxhx.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gkjlgqdec.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gyatnevct.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gtjxcooqd.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gwzwilncs.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gqfzujcmn.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/ghdpidxtp.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gyojbyluk.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gsbcdarex.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gpothtghx.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gqtrkrbyq.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/ghdzcdnjh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gjoicuemz.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gyqmwahss.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gunakuhmo.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/giplggacx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gaazmeijg.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gpbickkvi.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gfkjzljyp.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gcbcfkjns.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gxmibbwiy.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/ggceextgr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gfjkuybqk.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/ghmmjxtbj.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/getgftmve.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gwjzkwjgr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gicjcykpz.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gyrntfjcq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gkeafeepr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gzevgvmuf.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gkpddrfnm.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/goctkscdf.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gpaidowvu.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gnjdigbzr.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gmvjtlnut.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gwrrbouth.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gdkpiaqya.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/goshjttjb.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gcfhvfrpo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gyfufbiez.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/glasjmdbv.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gcrkblscu.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gnmsuyosx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gjosltfuv.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gahijpkgc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gcpszbqng.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/ggpftjwem.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gcovfqisj.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gshsrbbsj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gupmtkzkp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gaftpuhhk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gxtqvtrlt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwtablljy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gdfipazpp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gtshpnalk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gnqlxjijy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gjeudymsr.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gecfsnytf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gibidzzck.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gepsfiyrv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gcauskzmo.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/grehummgl.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gfltepvjz.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gpaoauhty.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gfkcfdvre.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gkcrkaoiq.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gotjctoer.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gjtiqozqm.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gtxqgdgeq.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gnvwaxmhh.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/ghamutioe.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/ghtjlcywf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gvxskouiv.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gblpkyqzw.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gvbepngqz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gpdablpqm.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gccqiakol.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/ghgjhuxsj.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gtjtwgykh.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gmfwxsdjr.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gsersvwgs.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gxvwjqfws.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gsuvdledo.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gxrxipkyc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gzyahwtlr.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gcbrzamyn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/glmjmdkre.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/ggeknwcdh.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gzcfkqsyu.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gxbjeqbre.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gychvrihu.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gjivpmlsf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gefpcfktl.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gxoumzodw.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/grmgyriec.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gwishxhby.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gtcrelkfe.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gswxitgoq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gwylecjsq.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gxslwlcnd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/glikrqkfk.sHtML


<!-- 参考信息 -->