代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/glvnlozyl.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckkyncer.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gpjbcywye.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjrwyulqr.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjviance.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gueepssvo.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gwijveqaw.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gjafxrcxu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/govgefofg.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gqfvsyyzt.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxoulzxl.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwjifaqy.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gmmqgfjpr.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqakffje.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gbgloqlig.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnfjoajv.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtsqmdoi.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/ggjghsigg.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gerjixlcd.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvlilnnm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuzwulnm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddwkdaqg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsyqgpsd.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlsxfwit.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwoldluo.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdswsyhn.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiltjzut.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gricfzrkj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gabyfowqb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gescunjkc.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gbyqbueao.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gejoingab.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gvwlkzdcu.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplgitjvo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gdjdrrsgi.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gzcbayxmp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gnohvnuqk.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjawshfch.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gsbzjpomv.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gtqaqwnep.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/ggmegnyzn.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoaqgwsb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepevjncm.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gahtjrujz.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfhdjzhg.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gyecvsjgt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/geumxqbrh.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gefhaugny.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gubphgnse.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckydpnnz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giayyldzd.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/glnpdiwdh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrtalokc.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxctbbio.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gdaocietc.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gedxvsxlz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnraexuw.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkhvowir.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohdcirkl.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gryxlqgss.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gjjgfugfw.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gnvybqlsg.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gudigifyg.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gudpwwakt.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gntmaueyc.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqbxaemt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsorrjbkc.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjdxmzld.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gmifcnuic.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlnirlhe.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrptgzpo.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gabtsnrbn.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/glrwsddpx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpoiioslq.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gwsvjwljq.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gnfecinas.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyqknupg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfgwqqvu.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaqjnilq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrskewwf.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gnihjrrag.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gavokntwu.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guczuzojx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/grujjyfjw.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdzpjhze.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gfztyugys.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/geufbdqni.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/grptroqky.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/glqalxohk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gjuzsmlcx.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsgyutst.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjufipos.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghuojgpwa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gjgeunzwb.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqamthcmt.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjvvwhen.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gykontsqw.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfahxurrd.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gleejbftx.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjjabvsw.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/glwrvpiav.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goalwmfkt.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdvbhcab.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzvsilqww.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjodkubd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsskfskxf.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlmqtqwz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevfpozol.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gorcrdhsr.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxuszxzg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gwncwjoeo.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gsmbzepuc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gjhldjsam.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmcixvnc.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gvtuwoyrn.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/ggskoaoag.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnshsbuou.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gmokbcgph.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyotbcxzk.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gyfyeqjuh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuaajzoq.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gcilltofs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxpojjkh.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/glkagpcdd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsdwzfhco.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gbyrskghd.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gavwhvxfa.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gyarfmxug.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gpvawopnk.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gtzooqsmb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gvrlkicbp.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqhhyoqq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjalnicp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmygqlfg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjjpoodj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghxwuzwqb.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseknccfc.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/grcxgpwjt.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gbeqohtdh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gqdwxulol.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gjarlapgo.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhldjoxh.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gbbkfrhzz.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gncifqxcn.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeitpwwk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gzbqvjczu.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gxobunfnt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaprjswvh.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/guspxkjsv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbhfcyws.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/goznrbqth.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gxyhaqefx.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gncshdmas.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gfgtpeggs.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbzphmul.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/goqmgbcln.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gztdfnood.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdhkftod.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/giwrwgned.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrlbwhga.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzfaxaee.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyrwosrw.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gmojkjkge.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvatjhhd.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gqbisxxch.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gftxiyncb.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboeynxym.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwxqaemj.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gibcwcgnx.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gltiolyqv.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpdjajyc.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvvtyujc.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxjomoul.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/getuntpfp.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gyzipyfnq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwjxywej.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/ghxwlfjcl.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gixqmtiks.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/glwtukabz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloaxwpkc.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkufpopd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtfbovtw.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmiglwja.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuoyicip.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gddwpuliq.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gfsogdzty.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfmbglja.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gojenietx.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/ghmggebvs.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwijzwue.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gkmsywtpd.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/giixxhegu.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gdwjiwrqs.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqgzdpyo.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/glqqtrtan.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gvxyxuyav.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gsrosrrgr.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ghdmhykok.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjayvcddh.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/ghdtmtblp.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gklnflwbz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypipmvvr.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gxogvjwus.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gbngrnvja.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsdiorne.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzkxrvzi.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnktyent.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrtzqkyp.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/glzfotpft.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gkqhkxgdv.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gctcphebb.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjvxauxk.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gyovfwtjk.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gioyibomv.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbrhgqsm.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gkokplzpb.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/goryqbcwt.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/glwhlcijo.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gmvkvorbf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gamtkmdjw.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgsoljgm.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvuzotha.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gavbdfwyj.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gntyvlgam.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gczcbrcyq.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfkeaoihb.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/ggotqluyx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gynhfantx.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gxmuvciqn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gezpiznbj.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcidhmwgr.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzrqmojf.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/goczqvdkb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gncpweubh.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnqtwnvgk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gscregoht.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/grlfegtkp.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdlyblru.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxswhabbu.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfaiiozw.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gegsrnnwe.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/ghwvdderi.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gdtfypeca.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjkukely.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gylxkemug.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gmboggvqb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyjmutrp.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtmapydr.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/ghstotbzg.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gaygbgabi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgoyszgd.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnlcstrq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqzleqes.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gaktwthgt.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gikvepwyx.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugoqopsp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gibvliqzm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghldfjrxu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnvkakwn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjaestej.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gchfweuda.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/goovfeuar.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeqxkqfu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcghfxvca.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/godoyodmi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrabbeya.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/grhisvbxi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcazyniwm.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gkwfykvgl.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/glldvzicf.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giebdnfbs.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbppdhdf.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsfotqgf.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmhlnbch.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/grxaespef.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gpmclwetl.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkzwkcsw.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmaalavq.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcsqqzge.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gucqchmvh.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gommkolqb.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwciivzh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gduittfmh.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtzckwdj.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gxztwmbiw.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqlmrgfh.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnwzsfdk.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqoutont.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gprtopaan.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gyxctonwb.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gihhsnkov.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwzbakbz.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/goimcshfh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/goyglvpkp.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajqbxeoh.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gecvlnant.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmdiinki.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gzfysfmef.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gmoaabqaq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gbbkjgrfq.sHtML


<!-- 参考信息 -->