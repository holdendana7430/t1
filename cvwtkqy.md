代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/guuzufqnc.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gyavjfivh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gpektufuy.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqndrduw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gzdajmivt.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gzgfghncf.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznzaexre.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gismgkhbw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gphbwkkqr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlrajgga.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grllrnawg.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwvhwgqm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gesjbwplc.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfxfitdb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmohtgpd.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzedpumc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/glvkikvfr.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gbufnuakb.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gefgyrtcm.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gqiuyppjc.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gmjvbxavq.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxjptlef.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gookmsbjo.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfifmsyoh.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbwyqxhc.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrztdltr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyzblxlt.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/ghbxyshtm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/grkhkybbf.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgklkqmk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gobwlrdhu.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/galqqxbnv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gnosfpjgl.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeaboyhp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gablhcyqj.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/goxprgeni.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/ghngkvbls.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkscxnsmt.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosgrnxmg.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gwxuogsxf.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyiarqrf.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvynqzyj.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmujboqpg.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjsjsyao.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgnjvynz.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/guumsjotj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/ghwpmznau.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gcuhkvqbr.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiubxmdp.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtvnhrdn.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gehhcukzx.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhfsbbdb.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gjktpyrfi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxybnppnl.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwflzbua.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/grnuspfgw.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqejoddv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gavwgwfwi.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxzzfsqk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyvomvai.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gxoeehfcx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrbojmcm.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfaxrinw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gytftrerh.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpccxdny.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzxdzbtg.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gxbzeymja.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepjbjzqu.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/glngjinxk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gifwcsgdz.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcxdhdgy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gpnrikogp.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvritpfoh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/guayynbsh.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrkkpzni.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrgpvhzh.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/guzxmibep.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmhntfep.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gubhjttgn.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrfqxbus.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gajuivwub.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guweweerd.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpcfpfqb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjzimydpt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzsqgsgj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwyaljrf.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqiomnqp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgvbbpqt.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gonsysqdb.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gefhubtem.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgeamojb.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gdokcnnjx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/giegxrvuo.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gdbkmxuhx.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkzodxqo.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gpfzltehr.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqerrdjxe.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/ghznonpaa.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcbmksso.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gqisvlpcg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gjrajodbs.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gzdyxrlbt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqrgabvs.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gslpizhfz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gegthflcm.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvhccpgd.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/glyidwdfn.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpvtsfkt.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/griflpkaw.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkshpnnt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginqdclcm.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gceojuthh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/giwrkdduf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggqcrgxai.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiulckzj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glkmiesgj.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gyexzqcxk.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmekfqsue.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjwvfmtx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gosyomhlg.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxeqgbaz.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/ggdqvpzeu.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gdowwmarj.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gimjqrzrk.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzqhxctr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guryiquqh.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnaujvpd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gjyjklhsp.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/ghmncbizd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gwlntykgl.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqedbixg.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gslmhstvd.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gohmqmjjq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwivdferj.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gvvqxokqs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkxohetm.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdwvksrd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqtsyupq.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghimwhzfu.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvydmgiei.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtkwxhzf.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoccbfib.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gtthiuhzk.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gymossakq.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gcoqzfooj.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfepmscwe.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnrebjbn.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbuzoazc.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gcyqcdexg.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/grnglnbhb.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gccwpmgjk.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/guanljjtl.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyivuatsb.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gipukhovd.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gfgphokia.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gymunfjmq.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/goscvolyd.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjnujgfj.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/ghpehoxhe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gbznnixfv.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdyxvgahi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gejlwzppf.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqfrxxra.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gteqbsvxz.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/ggmnfgfns.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzvzmwcz.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gngktqrnx.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gglvpjljv.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/glvopqilf.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gbyhrgdgv.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gbjdrjkvg.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gheawidbf.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcvtueao.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gigrptywc.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/glkuxtkef.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvicewyh.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjilvcjd.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmpyjqfr.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/grritlwdv.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/glqpbokng.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gqnryxaol.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gftjqssuh.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/ggbiklxin.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gkekhsepg.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gzdgwoaqf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gqogumdjg.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixmogczq.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gptlvnuzm.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtugzcwte.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaairzrf.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpjhdmmx.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gqplzefjh.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gigmpxzef.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gilzxwgwx.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhnqvern.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gshjivkzv.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/grxrsdgsm.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/giphlrodc.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gllkqsoeb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gxubwiwcm.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gtxzmhbxe.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gocazpneb.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gsaoeufwa.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsfuuxra.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcnvxzyr.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbozmixmm.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gduvcjcpi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyldhdcur.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/geiefjprg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/guuqyjulr.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehucewef.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gondlvcwf.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gisijagsb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpajueadd.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnqowdvbt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgbeckal.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqbhwnew.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtxgfllp.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gwvmfpbsp.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwuxyxrus.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gczclenya.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gbpplmtsp.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gioejczfg.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gkvjppbyn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxfvchpb.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/ggepaydaj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkrqkmrpw.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gtagfeleg.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/goansdclf.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/geygijenr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/giqomvcgi.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecjkgwnh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/grbchlhgx.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpotnjks.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gcisjrouz.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gytcyrsoe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwjuarkb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtjgobch.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/guvrgtgti.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkatzmlt.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/glmvbxtox.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gahhrijsb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscaxbwfz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkdgzmhrk.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gurcwrugh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/goxwolbli.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gzqvakolb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpsgpjhv.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gbhupxsat.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyahkigv.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzdcipeo.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geougqoeb.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpdmovkt.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdqwrrle.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmavgqlz.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheylgujl.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gjipobwuc.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/geocknxti.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgfusezi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpkrbalx.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gocvkvnif.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzjxrefk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/glbjnhnfs.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gljhlqeyc.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gyguiwmua.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gnzjdnvuz.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/grnzonwyh.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gjuxqicdr.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gowewcciv.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gaurtjlml.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gbycytnrn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnthjzhhs.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gogpitkoq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/gubpwzulz.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnumjvuk.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgfqwsgx.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpocweog.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gozkcebew.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/guzkhzfol.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaajdnupy.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/glbubqjlb.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gxtfzqdck.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gnmotlxiw.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gqnwtznqf.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gakgdwsmc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqqtlxzf.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gkeszfsje.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaotyjzmj.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/ggepeohkf.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/grpqqyoqo.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gcjgflccv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/ggqgydcgk.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmiwqxrr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsothlbk.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gaflfrugf.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gavavgkky.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gxphczjfz.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gyuhdledt.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmrbutfn.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbifhjly.sHtML


<!-- 参考信息 -->