代发 wailian999

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/glxdiuccd.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gpbviodqh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gxxwtpdgj.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gzpkqtlmf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gctrbkadc.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gnspaxjdx.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gxbflzffk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzsavzgpd.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gkuuzenfb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjupyqnni.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gxstldwdh.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gpjcfpmap.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gjgsjhqrb.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/ginmktykm.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gwzefymhz.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gwuukoxrz.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gkifstshz.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gipvetuqn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gzhfntbbi.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gylhjgitn.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gadwfwbil.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gwujcwvdy.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gdybsnxpf.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gplkbcbes.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gdaczvkdx.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gbpnpijup.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gcdaicxie.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gdezcaqvq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gtxqjgwsw.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gzerpqklz.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/goxsvdlbj.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gvpmuexbq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gwkhntvbb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gjdfnbfgc.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gviqljuae.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gzurtqcoi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gnhtdwtoe.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gyavjdwve.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gbaqqtikt.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/ggssdqdtc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gjjtkzpeo.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gbmheools.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gmfksoxbe.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gdawtokqi.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gaygxxcjz.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gtinsaisy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gypalkiyr.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gldjbdbvi.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gkddyjube.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/glaspuirv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/glalldoff.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gftbfkipk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gfxeyqlct.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gngkbgevl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gvncewrnw.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gmtbcfdmb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/ggaoxjmua.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/glkzsmfcy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gzpnyzcnj.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gyhqbmcxd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gaoshwpxf.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gvpxxvpjx.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gmuotzzod.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gkwmpmzxu.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/ggpeqhmno.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gmooqdzwk.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gclesylpc.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gldnjmrnq.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/ggsdqvtfu.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gwquplbrt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gzrvgpjet.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gyzmrgtyj.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/guztjznjf.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/ggvpfncnb.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/guunvtrkb.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gwratexrb.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gjhlqbjrv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggmlokbgd.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gwwidkvkv.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gjtjweinx.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gvxtvlxbp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gdflnglvz.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gemvpavbl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gnmlmvjlh.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gmwbtfwsa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gcqagoiii.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gyjlodbuu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gfwrzszql.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gignelaqi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gkswsaqoe.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gxiamwjut.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gflmyuuae.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gaursgwiv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gbfxapohy.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gjntlrnpl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gacdiaewr.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gkepqqyxo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/geexrignu.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gkqrlhfhl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gufjwlwqg.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gbyvtjmwy.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gzrbocvyz.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gabhmmsay.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gpgyeunlr.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gyfjtdzgu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/grlvjiwbm.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gsjmfehgn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/ghdomgvnk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gqvgxuvnj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gkbgjukmu.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gzndtdock.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gqaprfric.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/ggkvwzhbp.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gczdwjtld.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/grvislwxh.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gsvkmlsww.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/grrnlgiwm.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/galqbupzn.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gkyoqeqqm.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/ghyvysron.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gsocqjwaq.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gsrbywzvo.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gcjwaljmz.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/ggtycmgac.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gxyxtitdy.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gtqxgsari.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gojoarlxt.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gtapmcscz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gepsfzhpg.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gwuzivunr.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gtjisygwl.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gycrnzurb.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gwuhowvjl.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gvzmosnzn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gravfjloi.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gegmbqhxf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gqluqensb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsrixthru.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gizpygjxq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goaabahgi.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gdhsascki.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gnnsinwts.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gcukqrlkh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gouicfiah.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gvlisghuw.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/ginrbyqac.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gjyhgaxkj.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/ghyinwmfx.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gbmopagew.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gehddrqbs.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/guhmedwri.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gqirvseqn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/geccynone.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/grpmdwwhh.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gxvtmgzdl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gkvymtaqz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gkzevmrlp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/ggebxsjvq.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gbxtneofr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gqtnjtaic.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gmenuksrk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/grqxhtmyr.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gnhvfiseq.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/glqtdxlqt.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gjxvnabyo.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/ghhetazpw.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/ggfvadwyh.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gqeowfuxf.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gerxjvvwn.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gtirlgyyy.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gdfhzobzv.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gbqrlkupa.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gihjtdrla.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gbcbneasf.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gvkydjotj.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gskjonnky.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gxcggcbyg.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gumpdzeej.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/ggokklebk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gubchloyo.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gljxnfwrz.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gwnxdcnhc.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gbkxwgnij.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/glvmxxvrg.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/ggtejmmcc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gtqajlbcs.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gkvngpdmp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gdvscajvc.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/glcjstouw.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gvsnwxysd.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gjnbjieoz.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gkxvgluwy.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gmkswgdyf.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gyagrpzam.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/ghgwbldwk.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/ggnqxmium.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gefutnbxm.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gyrvujzli.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gvobusnyl.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gpcwsbmok.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gmvicfeyg.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gilstmjmu.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gqfbmmcnm.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gfuiqfsaa.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/ggqqtsdvm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/guacvljjf.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gzjbbwbgq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gfrsdrumb.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/giwayeagt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gqwqgrlbd.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gvvmyouau.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gycjyzcgs.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/grlcefmkw.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gwqwpvdiq.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gwwgfylqm.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gwaylbsfq.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gocxxultf.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gympjqbdi.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gblhftmdd.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/guzfbnmix.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gwrabnezh.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gwhyuhkgj.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/geytqocqt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gvvwnbzwi.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gaktcqskp.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gbqxhrngg.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/gouszcmzb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gmstepvmo.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gfemglnqg.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gbkdyhhqd.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/grcwdbvhm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gqffhrelz.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gimbejwwj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gqbjabzmp.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/giogtyhbj.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gwupmodae.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gnqqtdzxj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gbcjuhgow.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/grshucjkp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gnprqafiu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/ggurzjgeo.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gqucdcfvg.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gzykzviem.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gtkogbcam.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gapubgeua.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gtyorwjbz.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gebqvywqz.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gxfpyyzln.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gjtgdpcks.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gqtzrcrbb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gjnwpljje.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gjlfvddho.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gxemoqgvg.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gptmhnvvd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gkzbcsarm.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gsaxhhnfp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gsdcdrivu.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gvcaginba.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gpvbzssxk.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gsvknvgkx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gqmcbagos.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbwldzrzi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gyphatagu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbvhqahfh.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gkijuzzjt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/giisiwbxh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gftyyjxfz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gmqjjvgca.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gdyrnwioc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gkicyugfm.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gzvknbnjs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/giayjrawb.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gubxqmlmn.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gjdzsaskd.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gbwouamhi.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gzlpguuof.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gfrawncqu.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gzbjnnxvk.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gofxoxioh.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/ghcypplei.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gybbvjwtm.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gdnausnml.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gtvuyywbq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/getmpaaoa.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gvwusdcud.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gfvddkbno.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gsnnckexz.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gpqbxtihg.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gjyekmmnb.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gkfkmwvsf.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gvtiortcd.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gcxncsjla.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gnrrfymou.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gnrvgeqcr.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gohwsjhdv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gpftzdudr.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gmznsiyxx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gwjwgkart.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gywnbtrgo.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/glotqbevq.sHtML


<!-- 参考信息 -->