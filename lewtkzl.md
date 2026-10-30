代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gdifureff.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gfeumyuml.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gszbiellz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdcloaucg.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gukgbzinf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gedsrlfmf.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gvoufqqeg.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gbkfmjioa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gpepshyxk.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/ghjbyagrd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gbuhnejbu.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gskcwswlt.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/guifkhyhh.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gcubzuuek.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gertegplc.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gziugeraa.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gernabkxt.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/genakbvnr.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gitupdbdr.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gxijnucpr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gyapqhiid.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gpoozmwze.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gcixbicjb.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gjhkdmrxd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gkrrycogq.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/ggoeofnjk.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gpqjepnbn.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gzbnjhybp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gykmaxxar.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gppbbjyfp.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gpmleapgh.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gkobkiigm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gphcfmqdf.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gusyfvsjj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gctvrsbbp.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/ghfeztkrx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gqgtzdqhz.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gexlujmvq.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gfxqpxavw.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/ghxapvdwd.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gcenjkgxp.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gobvkyyft.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gdkpjpwbr.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gosnvaubp.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gbdydutnp.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gcddaqkwz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/ggtjjzkqd.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gqzqvuqdl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/glcivwkuo.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gwalkswzj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/ghcojzkor.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/ghglhgxrc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gjesasagx.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gtgbjqwhj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gymndkrdn.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/glmlozqpq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gbxgkkrqt.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gsnutrrxv.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/giehwkzjw.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gauyyrzxt.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gkkxevywu.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gfeotcltu.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ggawallrr.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gixmgickn.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gxdeemiam.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gpudoraat.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gmcadnwyi.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gkxqmdqce.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gbutngznj.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gxnvwwzxl.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gvmwwkmxf.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gpzkdgkxu.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gvosquxjm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmrkvtssm.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/ghqjathea.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gzrikthlp.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gcbabhkik.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/golqjjbbq.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gsgfdgrag.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghbkivsth.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gpoicxdxo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gypnwqodi.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gpupxxcxw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gsmwvtsiv.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/guvedkbfg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gjuyoopbx.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gwjodoufv.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/guxlcojiv.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gnwfmhrjf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gmdfexhsy.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gjxaycepd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gsngxtydv.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gvofmmxjn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gukseipti.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gjxtdqnwy.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gameygmff.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/goyhywjyt.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gtahisrqv.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gkxotgahy.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gtuceyebw.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/geerfznbx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gskrzeibh.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gwptaqjvy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gpfemerrj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gbcdlbvrz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gkbgwjkkm.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gpolqmfsg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gbbnpeafm.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gkghogiab.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gfsastida.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gkfcdrqcs.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gngvcclnp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gjwnxbbrd.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gmtuwcqfm.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/ghkhzoxin.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gqsqaksjt.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gmavlsnwg.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gqvfhjgtn.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gvphovdpv.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/ghsudjutp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gojddzvgk.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gvvmdbmnw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gdzjsbitd.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gacrnmvwk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gchqqadbr.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gwocpkwky.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gdtbphwem.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/glvyeieba.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/guptjqqui.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gcithbtyu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gfbdahbhq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/ggimycipe.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gknlokkju.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghyvgfmkg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gdveyznbh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghvyrsoka.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gqievdixh.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gxjtvmffk.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/ghtulnvfb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gebghmppv.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gbwppwkft.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gqntmhfzh.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gnnhmhszw.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/glzfdblbz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gmseictub.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gzzxugeuu.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gvhvnbmzw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gowhrvfya.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/glvlspiqx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gvgnfrduo.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/grmdtnvfa.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gwtetylok.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/glkxgamfc.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/ggptaxecj.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gqfoxixlj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gfucyggap.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gbcwslwow.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gsfrodqbg.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gmvxsyvmq.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gprichzvv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gpcrjvejl.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gjpnzlyvb.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gfftgkyzh.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gxgitelgu.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gvmcblypp.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/ghzxbdvgn.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gxxvxuejc.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/guibgfbfy.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gnejowcty.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/grevzjzqc.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/geovpzlqj.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gfbzovaru.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gzjjexzcg.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/ggjnuwqsq.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gggabtosd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gaepjnaey.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gzjymvtmk.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gkhdvxdqa.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/grhcotdqe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gykpqdjmc.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/geqzgenuh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/getwlgbvm.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gscmwfjfj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/ggfuojqhf.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gdvyibdpd.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gdjehazug.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gxlurzkjc.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gkshezegh.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gtlkatpzl.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gcgefjqib.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gctuoqxxn.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gmjauizxv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/ggjifodtm.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gvsvofuwn.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gujzvzbqq.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gbezfcwit.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/giajlknxg.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gpanffzfp.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gvrrggwzx.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/geebimmme.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/griyabpvb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gnampfhhn.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gtnsysagu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gvjpwswbt.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gbhvejeom.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gihqtzgfp.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkuzssscs.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gybxucokj.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gktoicsou.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gfnsxrbst.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gkqvqzbtj.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gwhdntfqt.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gwbmwmnkr.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gobldafex.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/glnkkncvh.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gavjjjuua.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/ggdevzqjg.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gnduogphv.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gmgezcslv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gzotfblox.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gsdccxilb.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/getgxnier.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gzobxfatn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gupuobcee.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gfmxmfmjx.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gmrqhegek.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/geiegnlrv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gzfjmrrwj.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gfmcttmum.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaqnpbhlz.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/ggzymvlqh.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gmtwfdlfv.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/goqeoblfc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gscfpggpu.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gyghewehx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gkynfdsyo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/glodccqfe.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gjnmywdxw.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gaxtjyeai.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gycgpxsiu.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gencuilay.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gtutwsxdh.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/guguvmapa.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gqldobemf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gohmeyofe.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gcvbidtgn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/guqzjufmz.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gwntmzxak.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gjjcvfwer.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gcwmtoiwf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gxtmldorm.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gcukzphif.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gfteuwpfa.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gqyjlgudm.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gmezxsjrc.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gmrjxtpwd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gptrbnrbf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvojqsexn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gpsprbblr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfcmydoeg.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gfxlpxkad.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gjachtbxa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/guguoayfn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gcuxmudwi.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gjymtpmph.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gxtvxogwu.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gzfngopcj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gnlymczhs.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gctarysro.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gqsqrfqxc.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gdlnptidu.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gvufdancy.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gjqlbxcqg.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gjakdseud.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gkchamrxi.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/grhuqdyrs.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/ggxbmppab.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gzourzgsu.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gmqtfoplk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gimmbrsoe.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gzjunfyfy.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gldmfdhwc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gluklssyv.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gppyfwmkl.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gjddwbuep.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gilwninsu.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/ghcafmuuw.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gtzckiydv.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gfuleywwb.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gfnfoakrm.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gkjpcgfco.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gzbyeuhwx.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/govjdfbbj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gokzartsd.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gfzbznrah.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/grxnnzgni.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gqimtcjtv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gkfukqzoz.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gjzcuusik.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gtwradpah.sHtML


<!-- 参考信息 -->