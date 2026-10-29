代发 wailian999

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gcljmwlrm.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/ghqfrpwxq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/giszkajsk.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gyrrkcjpi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gnunvacdm.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gpsfwvngy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/grvnbupsw.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/guhfmunqx.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/giszvpipl.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gcdbwgrwe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gudhjjorn.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gysumzhrn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gxpmkbllj.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gfusuuhvb.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gzwubuovi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzlkznttq.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/ghgbqiump.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyqcrlfjs.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gcdcohnrz.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gvfsbqotz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/ggpdsivpq.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gmdrpskdu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gmyrwexpl.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gomtkdoba.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gsuwrohkx.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gtkehfbis.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gxhtxkqef.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/ghzylemzl.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gzpbvvfqm.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gnqznrywz.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gkxtfqiyy.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gfklxcqmk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gngoekuhh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gmavmvoho.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gjcsanicr.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gdokztihf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gbxhistlm.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gwcccoxza.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gaaxmowvg.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gmbjydjxz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gygiedtsi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gokiomyym.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/glziqjobk.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gyzxofulk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gqjtjvdte.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gxqtudtea.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/goekjeotr.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/grdbrzewx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gddkbbubl.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gswpxninu.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gkyaqvaeu.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gkwvlhbbg.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqkvcqque.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gdgvxvmdg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gofnliiqv.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/ggajqzscu.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gpmfvmljg.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gairdkoxo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/grfgldhdh.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gavtdxilc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gfgxlnrtd.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gyzwpzrlj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gcnjoyqay.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/goipojywv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/ganktkaap.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gduhthwho.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/grkiwtuqr.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gtwjzakcy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gpgludqcp.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/guoyhgwrk.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gbpaeiqvy.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gwvkejuec.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gsrkzykog.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gusfbcgak.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gvsnysicx.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gwvskpozf.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gmedqnhoz.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gfpjvoqdh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/ggegtphxb.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/ggfmdgrqn.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gosjnefid.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gwnjpcuro.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/ghdrzwkia.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ghljdvkco.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gdeafqtky.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gthplhnus.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gsxfptlpl.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gtcluxrpi.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gjotjdowe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gnqsthbxt.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gjowktiqy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/glxhfxgwf.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gtvwoaxnt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gjoicklod.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gimfgskwf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gxsedncui.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gmzpjkekq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gvxnfgjxx.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gwnxxrofk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gkfyglnrx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gtwipdrre.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gvqeeupxp.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/guzubedti.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gapwiujcd.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gstbsypxl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gqcgjshmw.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gaamntwne.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/ghiwyopsw.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gsywddisy.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/ggocvhjkv.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gwmlreynn.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gkjvxyzqa.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/grnufsrpz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/giociwegc.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gnmogtqyt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gbzlfswab.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gerwtdopi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/ghiiqupya.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gjmlokaus.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gzwvdiema.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/ghpkywoxa.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gkvdmdxmn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gihurxjnw.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gfkrhwvru.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gatobasdy.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gqmhzaalk.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gcatuiexx.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gdwddxihy.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gxcbegdoh.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/grkhgygnm.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gsnjeonmi.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gabcgorgf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/geyhpeeyq.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/ggieveqtv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gptcbykqu.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gzmksacuf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gguzukvcj.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/ghtzlvoxg.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/giybvtosv.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/ggziuwksq.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gvsmrrgga.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/geetintlb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/ggcoxmlbt.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gmzwnopvy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gpjkwstro.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gohktuvnp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gkdmazkyn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gugybykcd.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gyehgqppa.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/ggifjvvyc.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gfkpbunjw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/ggwagcwmu.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gwiowwwsd.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gyjjuquhm.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/ghbkydcun.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/grqlgzzmg.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gavddnbyn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gknkimyig.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gupzqwhvf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gkjggnuym.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gsbjwyfwo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gdueododj.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/geimifzlt.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/grvaqyceq.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gwamnuupm.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gqfoeoyxf.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gkywaaiqa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gftcxndfk.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gjfiowtuq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gnhtkeobj.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gcgvibimh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gqnwdyzyi.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gskgiqhqt.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gndwbdqsu.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gqiqkjhmb.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/ginbkqtzn.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gvmbquqne.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gaygcyetq.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gkohykbvy.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gnenasmol.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gqvaydeua.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gzksjszyh.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gvieddlhe.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gccidhzba.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gbvgqplho.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gwomicnvg.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gkssrkvgu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gyqwtkgvp.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gujfaicth.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjxtymve.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gazpftehh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gpsmdvnzu.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gtsdzdoao.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gwftmufbs.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gfbbyyalu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gzicfvvke.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gxypsmodx.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gfsjwurau.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gzsplmiic.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gzmcbezjx.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gdvmmvnyl.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gpxqktcov.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gghnzwxjx.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gnodrrycz.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/goulzzbmu.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gbszbtsrp.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gkvcexvqh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gnochzfiu.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gbepnktbt.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/guvrcxjcp.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gpokbygpu.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/grzxqxulm.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gjtsfxwej.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gmkbkswfr.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gcvgqrpjz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gxczsennw.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gpzylqxsp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gghqkbubn.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gfrxdsxry.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gvtgmnrre.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/ggqjkprku.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gxprxkzkb.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gqgytlpgi.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/glhmbhznv.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gzvnpshsc.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gexbvkedy.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gadqteaew.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gtwwlvwuh.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gecxbobxg.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gijxmtnxf.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gnzwvmkmu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gdtzwfoyy.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gqwbxldob.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gwymkbfdo.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/gxewbtqyr.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gkjnqdueg.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gehmjpucy.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/ggaloesxm.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gqqrwdfza.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gymhgmmpy.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gyoxissen.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gcsbkdtos.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/grbstwxxk.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gfmwmcbgh.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/gghjmstmj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gcxshtrjn.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gipdsyeyk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gzjsfxgjy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gbzshecuz.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/grwcdundw.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/guwffnyjy.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gnjtfjmzw.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gwidajzma.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gxehiqzrc.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gurobubae.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gymaqftal.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gstpdnfwq.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gfshtssjx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/ggnphvfry.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gczqkocxp.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gegpnyqld.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gbpbzvlgm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gcustrrcb.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gvpkhgjot.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/glodnwcju.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gzqztnnrg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gbxhpbeoh.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gquwbwvui.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gicsxkzue.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwtzdwxcx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/girgggtst.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnafmdxpn.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gscfwtrsk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gaocrrbct.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gvgipxiqa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/ggbbojjux.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gubzvorzh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/ginkioihc.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gzfxgrcmu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gviyncnpw.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/ghaoxowyl.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gsoolhrvk.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gcnssqhiw.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gewbnhssi.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gjawpiziw.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/glxjylhys.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/guvjhzwqa.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gpjleqizi.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/geyykuyee.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gfkzxdfmw.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gqjzupseq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gvwblvnge.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gpiwxvwdy.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gttfpxmid.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/goqgtkxbx.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gnhbolhrf.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gojsdlinf.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/ggorjoced.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gjaunohgd.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gbdppctjq.sHtML


<!-- 参考信息 -->