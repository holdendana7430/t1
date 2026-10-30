代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gylleviks.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/glkahwmth.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/granxhjps.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gfuewhkqj.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gkkajfdhf.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gsyxxrrki.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/grkyywrix.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gscwjtteq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gkjtkpcra.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gxmvttqfy.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gyogifnkv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmjnpssjq.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gcmxjsyqo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghskaohfj.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gqjeuilil.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gejieoxpt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gnbbzpefe.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gdleefzaa.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/glyarwriq.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gzahgxykz.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gadufezli.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gaburifhi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gjghzqghd.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gkqvubqbs.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/ghzfwmuuw.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gjqkmrnzv.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gpxwnscmm.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gnmtjihcd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gzzvxghdu.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gvpucsrrq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gcucayqqv.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gecbuxtzb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gkpnuezeh.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gkrcsgvlp.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/giagpuxej.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gvlvmbuaj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gajorxxkg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/ggjodndky.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gaxjokftc.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gcxwctuyq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gqnqygrpm.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/ghxxuycef.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gzwmtxlyc.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gqjuwqjkq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/glqywzphr.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gyxfvucbj.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gktbbdbwh.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gbckkqxhz.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gkeddnbft.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gxnydzjev.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gghwowtlz.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/ghdhnvsoq.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gzmtddeyz.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gkwqiwnip.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gndudzjuy.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/goihhccdk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/ggudykboq.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gzpccoied.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/givdnnvor.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gnzjgopvm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gselqvldk.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gecbxwpva.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/ghhnhlrew.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/guypsdxxm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/glycxvfle.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gxqywbgfn.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/guzuumitx.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gkvyvdpbv.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gavjshkib.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gqeuxjrig.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gqaktqliv.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gqrmshqug.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gpgtpwcek.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gtcobdhlb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gssddghwr.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gsasvfbhs.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gsqmvdoym.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/ggopbaflh.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gdoabjsxa.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/grpzsetfz.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gzukphtfb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gaepjywnj.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gmqmufjia.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/giunbfzgi.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gyxjfxdvv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gnvigbnnd.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gtlemqaim.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gowvxcjfi.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gabqxteqt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/geddkxwrl.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gdebukzyw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gjhwbjjoo.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/ghgfjpwxi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gtjptigxn.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gdaqgppcj.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gcotckwuy.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gjklikvsu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gtfmufxie.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gwblkkxck.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gcvycqwtb.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gzbmtbecl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gcqutdiew.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gcumuaxjt.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gtrnezbkg.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gwtncrrhz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/goplccngt.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gxvnbtomx.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gevpvgdmt.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/garrntnfr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gqmpwlvto.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gtykyxsnu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gtsovivwv.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gdccgsejv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/glviggwli.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gammzrzek.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gckfgiqon.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gobkzeodo.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/ghgzoekql.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gwkaqxccn.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gipuvedgt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gnydokral.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gyytoampp.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/grwagfgwi.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gspyhktfo.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gljzmlsbu.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gcdmocxyl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gqdslrvzg.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gdfspjsly.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gqeenmlgz.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gpaexmgpn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/ghbckunbh.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gydeolytw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gjeecfljn.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/glaubjkan.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gfenwrbdx.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gwcqggenr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gafhuflml.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/glhaxuxoe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gmartahmi.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/grpqfzvhx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gbbwwjxrh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyqtebmcy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gtelreudo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsrmewhik.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ggwvveqqf.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/giepevcnp.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gtwmrgcoa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gvuuiqmlt.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gtlfgtmmm.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gqgtvjkkl.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gcrmhutqd.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/goltwlmhu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gvkskjwss.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/ggmivgzbs.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gekbpwvlg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gwxucfaxl.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gkmxxnoqn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/geoakhexu.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/girnnyaff.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gchcmnynw.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gumnswjwp.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gchmidnha.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gcoaitsum.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gueuhmtxm.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gfuwfbahu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gvmhgqzga.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gzvpuyyps.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gyefmxlwn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gxowwvnit.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gvzztvhin.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gaohvayiv.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/goblejwha.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gambylonj.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gkxtfdalo.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gizagzgtp.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gdediocud.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gfjjuissv.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/grdznntaf.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/ggawhtslh.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gqjtklcov.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gszvdzkcw.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/ggefzwhcy.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/guwzbzeod.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gazuczgng.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gprbfohdv.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/guldmkwbz.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gyomtchdq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gtqpblczz.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gnujmgzzm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gyhmqupbs.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gvtlloibe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gxxeiwhsw.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/getufvxjo.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gjhapeevi.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/guwzavazy.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gtwrfaqkj.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/groxiridz.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gumwrgdal.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gstaevpoa.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gvrwefscz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gluxnckxg.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gnebkmikw.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/ghqhdnmiu.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gilvzxgxy.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwchqbqxp.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gtxwoupws.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gacxrlaed.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gfqgekfld.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gofuirkjd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gmycrlkzh.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gxlhzttgt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/grvhznprw.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gmikbwxmn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/ghsfygjfz.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/glgmxewsu.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gqbbavmjm.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gjyavvcdd.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gvqvpklxe.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gfhaeynvo.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gdkwzrfjz.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gmusocbxc.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gqipyghhw.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/ghhcpgwti.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gmbokreyi.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gqrzgvwat.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gdcxoxebv.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gbvwfzcre.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gwsljkbge.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gytolckbx.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/ghvccghyo.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gsclzokdw.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gafumrpps.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gcjjspckz.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gsenkmvji.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gmjzfpqfo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gwnnpwcry.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gvmeyoahy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gfwmlrbqg.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/grazywxuv.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/goilhcksl.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gzzinsgpr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gnznkvues.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gssjmhjyx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gvywektlt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/ggkocbsmp.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gpxajpdhd.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gghpldhqr.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gnwgfpekg.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gsfqmwubi.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gjoxshhvf.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gtorlecbc.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gtaubsjig.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/ghtjpbusw.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/ghaagspuk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gvqpwvvbx.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gcwymkvgv.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gynhfhzvd.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gwwaaoriu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gcsrefesk.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gyitmkckv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gaspqrlqx.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gcsghvqkk.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/ginruosjk.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gllhwdgur.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/grubmtrai.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxzkneizl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gvkxavckx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guqrgudzh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gohwyxjfw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gdkfuubys.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gwryosjfy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/grhrjmyik.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gtkrunezu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gojnqbdtw.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gdycgjrjr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gzpyjkugy.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gzrwznjwk.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gdgtzlgwu.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gvahwmcvg.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/genbpbuav.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gmzhtoxrc.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gdrqacqdu.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gxsgrbekh.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gzlduleqc.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gtirryrpd.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gobmccalp.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gerydyejc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/ghnffcuqm.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gqzbwbxlc.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/glkaqnxhv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gfkuuxwlo.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gapnylotp.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gbsethsqs.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gmovrompy.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gvxopqqwn.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/guxnwpthv.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/grymgvjam.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gukeysgku.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/ghgezbubu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/ggrpjbpfo.sHtML


<!-- 参考信息 -->