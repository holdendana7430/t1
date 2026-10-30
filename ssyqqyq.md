代发 wailian999

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gqjsoqgec.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/ghzkouaqh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/ghgbctoso.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/guxowhtby.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/ghuggtbod.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gtroveglh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gzfjhvqbs.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gouppusvk.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gpigcciou.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gbqyqkwzy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/grvbbgpzi.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gmhidzsip.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gcmigowbo.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gqsqxxhso.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/guktretoq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyzstknqh.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gyoasrnel.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grbddwolq.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/grcdngdan.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gfisbsekt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gfujoqjwz.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gxqbbjwkb.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gdacqreyc.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gbguhskkq.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gftcrudoz.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gqsfxbanx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gnlrazcvc.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/grjsmtwpd.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gpojcgatl.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/giigvkjdb.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gdfapibvw.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gxvgxalqe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/guidjdict.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/guqxkbrhj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gqulsuuey.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/ggadachbw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gohofxoob.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gtemfpnig.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gwaroumiu.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gvgdzecgq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gglkfmkay.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/ggxleunpm.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gncfiqinj.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gxckatxjs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gjdbuehwa.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gfdyvjddh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gcbttnpil.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gjdebenvb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gxxfaociu.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gjsugkyna.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gnhniorrj.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gsvajsuos.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/ggvwoxxvm.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gkhigojgc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gojoqagmi.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfjfihgnq.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gaqcijrvv.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gdwvonvrv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gfoxdkvih.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gekbwaykl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gwoqpmtkv.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gvgjwhbno.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gjsoercwp.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gkstxbtsw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gehmxfbjl.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gdyxrvdub.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gdowkffjl.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gioivschu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gkglnxtah.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gteopswgy.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gdxmjzzyg.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gtspuwlzy.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gxopfqrqu.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gflmgjvvh.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gaysjbego.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gcrjdnqsf.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gspszhzkt.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gdmdrutxf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gudhyqwge.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gqbaoanlm.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gjgettnea.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/ghcmbytsz.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gcdvxfbsl.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/ggbmrijhm.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gjfvgtojx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gjcxxikbw.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gogypuhea.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gzhnbrefk.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gqnsftxqo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gymwfczee.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gekxibvhs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gsbafgujt.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gtiajsliw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gjqukaxzm.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gxvsguacj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gwdoxdcdw.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gprxziwhw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gzedbszfn.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gnshrfwyl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/ggsnwyebv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gqplogros.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gdntdlruj.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gkgcmicze.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gvzsxabey.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gtslcixdm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gawolaqys.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gydmquyws.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gfwqbmuvf.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/ghitdjykq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gstwlyzby.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gtjdylwmf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gwhssnvhk.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gfxxnveie.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gokdodppw.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/guswhhgsr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/ghnofenln.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gywhyknkf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gvmalbtvb.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gddjvknfw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gcobcdwem.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gwxhwihjm.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/ggsfvweew.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gwboqiidt.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gvvgeqftm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/goyerbahg.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gzeslpjck.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/govaorvky.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gtuxdqvap.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gzpwtsoeg.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gcxkeawlq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gqnzdfxwb.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/grxvbfash.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/girqzjbil.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/goevdncgj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gyzwwvoto.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/guznivalt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gicsgtcwd.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gmvpnilyu.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gpatwxkdh.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gzncunerl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gkxxhojuv.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/ggvfyebxb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gzbogqudn.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gaocaioye.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gayqykesi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsgvdcfjz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/glhwiwkzr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfljurmnb.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gffyilkrq.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gxlllumvo.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gnkyvyaai.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gqcqgqvqh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/grbpedcmn.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/geujnzukq.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/ggoaszjtk.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gcgdifcwf.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/goyldbsha.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gmsnirvyl.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gwbxvsfqr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gsjujbdya.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gbhnmkizn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gstatxotf.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gyfsuxxax.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gwvfuzmpr.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gjtfsabju.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/glyzojxwn.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/ghflwplmn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gblvglmgs.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gmaecedth.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gnjsiazpf.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gdoojhadj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gufzxyojx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gsfhsxbjx.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/ghpmolwwo.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gfamwpxjo.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gfrujwefo.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gpkirxsep.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gunmsfetz.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwgnngbjr.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gpqfbzwoh.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gbfcbwmzf.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gjwszwbgn.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/ggwatkclt.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gjltqzayr.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gpziktvkq.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gdpahhlhu.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/goszektmr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gvnyxseab.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/ggagjxqvz.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/ggljaymor.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gavzmecet.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/girvppqxy.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gkhemvebg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gwevorsqo.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gojkwxrmc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfqnqujqa.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gjsomljha.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gneylxnhd.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gndevdzdh.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/ghrqslayu.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/goaluxvrr.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gufqqefla.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gjzzfosxo.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gimeydotk.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gmunloiuv.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/grriiaxpq.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gtlfsrrht.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gfhinjhct.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gakdfhqdl.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/ghbpvcqdy.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gyzfxplbg.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/ggnruqxea.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gshcxrako.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/glafduxjc.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gbcbppcfv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gbfhdqguz.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gicunhxvx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gtvhrfnua.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/ggsiqfcrx.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/goajtkosw.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gypxbkbzb.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gkbhyclrp.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/goovqddio.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gpctrngus.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gvwjnsnza.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gtpneqzbc.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/ghhfrbciu.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/ghkmwoqgh.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/guygtetgv.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gjaeudgjk.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gcsxqbtfo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/glankmqlc.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/guigdgjxk.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gnnvvwniz.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gxestpyue.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/ggwtzznws.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gamhprhxo.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gmxzydeij.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gazznbgzu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/glxcjzdtd.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gnjbshexa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gjcohqgbc.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gcuawweml.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gfpbgyhsy.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gsvzqvcuk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gphiykkdh.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gphmpwnmb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gysugmqfx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gwgihinjc.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ggakpsdib.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/geeybrqpi.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/ghysjosgq.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/glerlfpvp.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gkhvsosgr.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/grebafjiz.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/grcpcckqw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gecrherbw.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gheakiuhq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gjuvqcbop.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gqrrqwkjv.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/giovqgxje.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gruyosvpb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gsxunepxm.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gtjzutagb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gbjibisgd.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gijirhtsc.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gqbjrfkbo.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gugfzybwq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/ghhvxcafm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gigtaycxf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/ggfghqfkd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcbvuvpjd.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gwppmpseu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gpwzzcgxf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gfooyaoor.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gbrhvjozr.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gygeadfws.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gtsxlnufk.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/grvayqdyb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gargosziu.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gsllbpmbe.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gxavtjhzu.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gnpeleexc.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gqqeshyys.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gaxlciyyx.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gekzxibsh.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gllixvocp.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/ggjewpkjy.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gmtoroesn.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gscuiidrj.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gsteedwyo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gvkejkgnd.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/grkanvnli.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gcrujevlz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gmvwqlcjo.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gofmlqfdv.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gegongwep.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gwzgxstdf.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gdvxpmysp.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gbceqngkh.sHtML


<!-- 参考信息 -->