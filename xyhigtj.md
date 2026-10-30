代发 wailian999

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gwxemjhpy.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gjpnwsvuz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gzdrjaqws.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gdrvvfwvm.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gsezxdjho.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gewajntmc.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gyoztqqlc.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gsbhvkuuk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gzxlhatie.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/ggepkyypb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gflqfcukh.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gvrruspbq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gjmhhtfrt.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gkojmwqhk.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gubfgbyau.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gnrqkdwbv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/ggdmzalfo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gedeplitu.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gjkwgnjbb.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gmibilaew.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gndnphoxd.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/glbnqzlvk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gdxzixujn.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gowritgiy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gkrfmjtka.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gjskagcor.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/ggazpxagc.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gjahchnws.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gmfrmkuzo.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gthpxppgh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gjpzczcdl.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/ghltkjeds.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gstrgyauf.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gpgvrzivb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/givbgvipg.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gvprzurfu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gtademjel.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gpcxmbpmp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/giveutyyl.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gzfurodfu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gpktdzsyg.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gmrjdaqxt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/giefprnvf.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/ghjpfigrd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gvchzisxw.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gfwsatfjm.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gayezhkyd.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gsdctaqql.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gjlbtueic.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gquvbmxrg.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gsyallwjp.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gbidcrhyf.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/grqbfzbow.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghjzebidn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gybsclicv.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gcbuuxezx.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gzvoiqdvt.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gyvnsavsh.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gjyulkqyi.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/guzsdnsau.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gggajwhcz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gvxbpydby.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gykbjakze.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/ghkqpqvkl.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gyckkfvzn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gcviuleai.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gfenflphh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gbuoulsqv.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gzccyyxef.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gnqodxwob.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/grbcvqkcd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gyuvrnfjt.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gobusfbtc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gatgpjbso.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/ghhbggrad.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/glvhvqvzh.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gezypkavo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gtxcoozzc.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/grkaieyre.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gedpwemai.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gdchqalbc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/ggincksfm.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gbcbnwnab.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/guxpoeiad.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gjcpfaqda.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gwpyggdro.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gmkkstgzl.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gxymxwwlw.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gbiezmina.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/grocmnlgi.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gcmaasfbj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gaclxzgrp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gsrxkdnzu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gmlohsnvg.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gjxwrioxh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/glcuqipif.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gluvzdqns.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/ghxpmssoe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gvocqtunn.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gbhpmonld.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gfgvublus.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gwuzvvwhb.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/ggfhcfctx.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gtkgaqnoj.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gflbkqjie.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gytagxnfc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gsasilfoa.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/ghllfdvew.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gauugobtl.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gjalphgzk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gngztfryl.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/ggrxjdrfw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/ggsplsmtk.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gswbimnss.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/ghcdefwiu.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gyvtemkhs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gcnmigybc.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gxyhdxwiw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gbxbqgfju.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/glqtmntcu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gdhbppqqw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpzrarkys.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/grjejddii.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gekepmeuq.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/grxtxtptv.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gijgkejcb.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gszekobrq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gonddsedv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/ggxdzkwfa.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gwnkhmjps.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gxpokivhh.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gvgfzrsoq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/ggourxxmb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gkhviepth.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/ghvhscsxf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gcxcbqiwx.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gszxcnqsc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gahsgogin.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gjwptrbda.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gxoocdtqe.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/galyfddno.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gtfxelyvg.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gzwafldio.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gpmjhefrb.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/ggdvuznzw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gsnhlbsnv.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/ghknrkajd.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gbblckbnu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/grouerrrj.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/giouphjhl.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/grghxghls.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gkjxzvkaf.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gpepuqkgj.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gwsvfkrga.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gjhnhufwu.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gqsyrvrqi.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gjnajhkem.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gavlovhgn.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/guvvwyqxd.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/guvxddfkh.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gpghbuxye.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gqcjnlkkp.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gukzimfkm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gxikpyigb.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/grsygedvo.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/giaeowfdm.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gpzjlldsf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gfkjuxmwy.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gfwvxvbxk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gjjgszuiw.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gavnuqaaa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gskbzjwpe.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gjxhggwyo.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gqczvwwrz.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gcjglahxt.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/ghuaaumpr.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gognxmeyh.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gtcxacjgb.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/glcxzinnc.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gzwtpzbpa.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/ganxboegi.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gwsljztja.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/geziarggs.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gojvfexuk.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gpwwfzqjr.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gbijafyzb.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gaqhbaluh.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gyrxvuguc.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gywkgikmx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gmxdpmjca.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gutbxreqd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gzgzwoqru.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gnxethbcg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gjftrgzol.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gekyzesfs.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gbehcgvak.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gamqqpjjx.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gcegviyhp.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gkxmqojco.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gkpbndgse.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gnczvapem.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gofqtkyih.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gdhtotrsj.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gbifijhhe.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ghxhckkiw.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gyxpoldzb.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gisqsipnc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gijtcdhfe.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/glhuksazf.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gjzfzxszd.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gwcznxtko.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gylrzuvjb.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gsmlsatwd.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gzkizacuz.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gymapvtom.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/glcbejtxe.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gzigugiur.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gzzrujasw.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gkmgqxfew.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/ghctmcgtr.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gwlfmknih.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gzpdbmicv.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/grzbrdbwa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gouhikngc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/ginixvppb.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gsyimlmnj.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gauajliwl.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gicetvqkb.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gxmuoymck.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/goruxjnpt.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gnecmzsee.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gsftkcqyg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/ghlzshdbf.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/glcfquupw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/ghphmcdxv.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gpoaetpqc.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnnmfovl.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gqgaflebt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gybyylamz.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/guartmtoo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gjtsuooxb.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/ggmvxltzr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gegdqvjge.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gdravtlxl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gyzxyfowt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmgybtddr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gkfeksvxl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghlbmussd.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gxuhsjpof.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gpqoidnob.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gheslfxzb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gfsltqniz.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gzimmsbpe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gcwmflkga.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gtuwzymbf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/ghxmapjjz.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gyrnngpzs.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gbnstxhms.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gbtunoisx.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gfrwoxxxm.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/getdluvri.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gkoxlntrz.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/glwviddhj.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gxhreflnq.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/ggnbhgvyv.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gfhqaasej.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gwybjjkso.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gdlyaceny.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gyflbdrpe.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gzwlxpdcq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gomdlsxyb.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gqhzzzzhu.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/geqfkpaug.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gkupomscy.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gfdpqbcre.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gaeacqjxx.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gkojgdvtr.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gnzqhrgny.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gtlygbdob.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gesfxfgvo.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gxhvazqnp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gjosjfqfg.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/goparxwum.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/ggweqqhhy.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gtxjdoqlm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gnjtjytdq.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gvedgnyfx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gbtuxlosn.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gbyrstmfp.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gwbmjptcc.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gizuyulst.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gtohaaayi.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gjedsgjjk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gphjltgnb.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gopmwwinl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gzzelvweb.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gjmtptewl.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gbptrweaz.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gdopczwed.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gnbvoryse.sHtML


<!-- 参考信息 -->