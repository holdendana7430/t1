代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gseruspgv.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gaqvgyiyv.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gxoptreoe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvwaudtzc.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gtasgijnr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gikyoygor.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gepzpdyuc.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gzzqcbrgp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gtgsddmel.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gomjjrstu.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gpfiszfrd.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gzzocmbbu.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gftjlsevk.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gdcftckwr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/giirwlsmz.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gmgwagmay.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gmaxfzzrf.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gvanjmrfo.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gdjvcwynv.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/geasuoxhe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gfkmwzyyb.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gjdqzubpv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gfkrxqjzn.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gcoxjqmrl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gbkwzjzuh.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/glkvjhlqq.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gfgyswgsj.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gmxcotqlq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gcotkeeqf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gtrgfwltt.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gexouwikn.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/ghxgclxit.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gevraqore.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/ghuywdouv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gqkbmaplc.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gftegtcvr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gyhpgbelb.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/grugykftj.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gbbyivsyj.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gcpprzuvf.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gisjndkrc.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gijpoaaor.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/ghydovkqz.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gxrkzbjji.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gybpuwhwn.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gxjfjmesy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gvaxyxhzp.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gcffosevk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/ggiiqzbmx.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gnpetxpcj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/ghfrbvjmc.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gwxdfkbav.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gesdzkbqd.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gnqewtzld.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/giudjuixb.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gqqkcztbf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/ggjaudjqk.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gyokcatst.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gconewoiv.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gwvxdenbo.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gdudhakiw.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gsyjhxvsi.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gzntouwxv.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gopiuptnp.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gdkpbskzw.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gsbbtfbut.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/goiutelsc.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gifkmirhl.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/ghimkyetj.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gkoagtffh.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gqubamsdk.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gpvwckdkg.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gdnbhdlcn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gdrbvtwdv.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gthxpgkch.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/ghvckodby.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gyyfjfkeu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gtvdhqepv.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gkdtwrgdy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gaowdpeym.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/ghmkmsifn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gznztlmaz.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gqwhxsmnu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gkrlhnyqg.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gfaaesmzl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gmjldokuf.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gwxgrqdku.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gdfhvpyps.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gjhzalwgr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/geaepdhcv.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gakvbnweu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gaaqwykkq.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gxlkcjcqp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gxexcsmri.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/grwwpxmmz.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gmgbupjua.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gixqjeovl.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gkrthfyge.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/ginujgpem.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gggxjqtek.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gzghmcvqu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gwuuxfehy.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gttlonxrn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gezlnmmku.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gzehpiekz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gfybfuuol.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gxmxxejxo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gxtownmua.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gkssubivu.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gxwmizidk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/grftyonsw.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gfdusggyy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gebziikzb.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/ggxlihrha.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gxkswxldj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gcywfsuxd.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gptrnhuzu.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gvaqwpihc.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gbcxgakss.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gmhvxpqdc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gswkwnauf.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/guzzfokkz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gqqtjwazt.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/glypixxiz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/ghhkuqedq.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gcxpwiqrd.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gkilcwskt.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gaxwvlqao.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gwdikylsf.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/glufniovi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/geitjmquo.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gdagglwek.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/ghiwcnkdw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwbrmwvxh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gsewdlmsa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnqyyxwww.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gzypqhjrx.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gwxxurzwn.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gdibfduld.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gziykkpxs.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/ggysyxckm.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gehrxdbky.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gaglbqslu.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gpzkymwku.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gpgrzdxog.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/ggezkorjr.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gukrmasbo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/giylmbcxs.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gbmjefpmu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gtzmlcqxk.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gfogzcbxv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/ghurlycxd.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/grlwtbxas.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gtsxtiqyt.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/ggcoycuvn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gupivoxpw.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/ggqigusqu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gecqavyqa.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/ggiqlgrjl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/ghqamdfog.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gdzbielzl.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gknykwgao.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gfnpdlknk.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gwfoavsas.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gqmaytuct.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gwkxheujo.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/ggprbvqch.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gmhedtsxi.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/ghbgrkeet.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gykcpcxis.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gbppyuaab.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gemvvfnjs.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gkcenpuqg.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/grfrrvzpz.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gepzobsfj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gjuryvoml.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gfvyddwfj.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/geitorkln.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gijuplcnn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gsjuwgegf.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gyaffxujd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gtqobejlx.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gletvlbmj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gbjjaqrqx.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gcxxypwlh.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gveanbgop.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/ghsgyidym.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/ghyopindp.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gcvxqgobl.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gkiymtniz.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gzbfhajki.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gnptojrij.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gvkrhpvcy.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gyhtbnpep.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gcmxwlbae.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gklyljsbz.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gqnxjhmry.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gxktbfgce.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/ggzkhgchf.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gmnhsqycq.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/ggzpnyhbh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gubtjpqja.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gknnpxndf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gpnlwmudn.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gafcdttdk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gqyosjhlo.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/glwgxrbyf.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/glcdublly.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gcewhnddw.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gfshzgjvy.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gpuhsnsal.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gkmppdenp.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/ggojsktws.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gafkekify.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gbunmavfs.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gtaupqmrx.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gqgyuqgoi.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gnxnpzlip.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/glakspqok.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gpmgvtgau.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gabptezzw.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gnudiwxuu.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gwwjssceq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gnfjfdkfp.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/giapwhcoz.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/giliqqzae.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gcykvvhrp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gfpkrzhau.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gnbpwplvb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gkiqbfogc.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gbztbnhyr.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gycgmsgvp.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/gihhhhpns.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gxefrfvlt.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/grqgllwpz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/goqzkbobb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gntxvkoqx.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gmvgcstca.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/guesnvfhl.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gsbztbwrs.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gnccgicpj.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gpphldyon.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/ghadoekoh.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gefezfvnh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gbqfcqfcl.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gybnqlgrr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gozpxeuxe.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gwgcocvef.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gpimmkxjd.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gadwlgznv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/ggduzmriz.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gqhewxdtr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gtuxtftoy.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gldkseuod.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gykxdsykp.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gcsjkiypx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/grmjszvjd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggkuhiabt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/goynydotr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmyrhosua.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gexblcobq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/glsrbpdzx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gemkhbqdg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gkjohneaa.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gtuojjrud.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/guxzujiby.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gwbtwkdrx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gkvuunydk.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gvurlxjlq.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gthnjszjl.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gjrlreesg.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gadktcdof.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gvcuzzusk.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gidwrihdr.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gnmqkxizp.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/ggfnalimk.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gttffjcwc.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/glzdawphh.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gwmimyovn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gnkscbmba.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gjbygatrn.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gxelcvouw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gdngalavd.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gaeccunkz.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gmzxqceqd.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gywxoietk.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/grjdcvxrz.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/goedibcfa.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gudeokwjq.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gwmklkiwb.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gseqfyvmg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gmqyexoxx.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gqwbdhmjb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gzkhfvkek.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gorrsiqgb.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gdhfodhsw.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gdvrksqgs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gpizgaaew.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gmegttnqu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gfluwcyjg.sHtML


<!-- 参考信息 -->