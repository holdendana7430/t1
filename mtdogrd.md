代发 wailian999

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gezbdmzrc.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgobmknr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmjloipvk.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqmwmjvuq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gauvyhrvm.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gajthuksv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgokijug.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gowjnawol.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/geszpezuo.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysdqrote.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmtuegka.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gelnnbeim.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/govcpcngp.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gcfzcmirv.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/grkagfkzw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gntfgnlsg.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gtmvdedqa.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwldvmuz.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ghdgsvgqr.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/ghdusfyaz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqxfcfyvn.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkihpzmvp.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/ggosphcze.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gybaykxnm.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpitckok.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gbfcnwabx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/ganfsxrrw.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gypzqtozi.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/glftuopvu.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggczzalzz.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gtlnwikrk.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gnaxkaqgl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/geuceuecp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavfrzspj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/glastfchv.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/goigdawub.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gniszdxxe.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnsmlhaj.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gwdciqenc.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxyzowzna.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gvxarlfnc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtupudirz.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkjkbckm.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gijijsiog.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gxjhwrjqj.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmxvbrlp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gmhsgowko.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzjrjosz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/grjudzqnb.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gurmvkpfj.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/giiuzdyvm.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gajtvrvft.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gzjrjevuq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gxqdkaquy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gtlrepsva.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtuyiazl.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmucmgmxf.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipjnaljs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/grbdwdezh.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/govnmfdht.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gibkbykkk.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gowqsgmdw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjbzjtpr.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gwiedebso.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsnbpdov.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrfkarlw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gtnqefjbx.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvmshzst.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gpmriwwzt.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/girdjjjjl.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gynqehabt.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gslkzsnfr.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqsrwuis.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqtomnjc.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpkkqpou.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gupctwxnd.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/ghqjegdna.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpvdzrhxp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwnmfhwe.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gjakczkoe.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/grlpjamdi.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujulmika.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gyycvpijn.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gbjaaofhg.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzjcfhny.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzujcqzgc.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gueabbeky.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gicancmjz.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsyvcuny.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/guygfbxfh.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gnrgdsmdf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghaddzpln.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/guduailca.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexiitjts.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxplksju.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gjmbpxdjw.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gifilvrch.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gcyjnerfk.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gctocimte.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/grmlxetxf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjohhsdj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/goivykxio.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gpichbcuu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gdumnkhhm.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gskwgpeje.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzzlaayv.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/ggbbgsrrn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxzadsyh.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gbtewnczt.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbctsifiw.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gklumgywa.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyeqzttks.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnbxrgmi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/guhmstzed.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/guiqtynbz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/giqzfdfpr.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gddbuucrs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gilxwjjtp.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpqsnklup.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmxhjybx.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmmbkpvg.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqeuoocg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxxgknug.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/giwhjodkp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrwyqqsc.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoknonug.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlaexqee.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyczekakm.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyfmfidpj.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsawgtik.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gbhupvdvw.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/godajwwyb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfditdrqd.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqtniwho.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gzprlzrax.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gpararovi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfjqkomd.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmbezhsc.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gqchcptna.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfeyyxxw.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gywwijkap.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosfdjafx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gmhnzyjer.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gplrwappr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/grghtlwnr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqncwzyo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gyecyejup.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnrguscd.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gfinlvung.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdjgxacz.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/geohqtxdj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gylojoxhc.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcpprbfc.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gmroknesg.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/ghjzftwgw.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjlxbtkt.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gbmzjqarp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gppmzglpj.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplbarjaa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gdxtwymzi.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvmuwhkq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gjhbnnghz.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghisdqque.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gfqmfewap.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwetsdkvy.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnfdykyd.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdmxabes.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gszvyvcwb.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/geqifqahf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhdxwzbn.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gvwwhhdxn.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/givycxsmu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvnsytzb.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmblcbbr.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gqwivkqtx.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gefpzoedn.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpcthhhl.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gpbyeldwi.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/guoeoobev.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gbkvhbpca.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gkngzzjpl.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gcxyymhuw.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxknmcam.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqzmzdza.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gbipayrct.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gmkjqhpop.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gosfirdtt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gjizmcdir.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzuvlxan.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gtznhndco.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gelbhjpks.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqxrvfxb.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwthriqsd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gznqwfyhr.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gnecwpaht.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gccvvstwu.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gjibsqwqf.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gbevlbvmt.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gdnoxkvdp.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/grdhumwcf.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfalhqty.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggakczrxv.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/ggqcvdafn.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmpzzugh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqewvsbe.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gysqrizqt.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuhjzwos.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydqmchml.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gacgerifj.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhzxshvg.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmlmhmbh.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gkakwifjj.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gaqvkiqhq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gcjfvqeka.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gkndffmrj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvntmgpfn.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywklrgdh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gvedxmjmy.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaocmjrl.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gusfdoclu.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqtengsw.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrbgljgn.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvofaenor.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbeccuan.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gsbnjfqmo.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzvkqese.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gkduufpaa.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/goeyoitiw.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gajogxmlw.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/goaarbtht.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvpjauck.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhuyaqvg.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdpnywjm.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpudafwh.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gosfcoipt.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjqhnbudy.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gpurphjub.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmptptyzq.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxxvyhba.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giblbcxyg.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gcypcmdzd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gboiqyfkl.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlotyeqe.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtefohtxg.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxifhoxru.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyvhfyyos.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/getxokjkn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gjalvihzy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glmzliliq.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxjovtito.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzwibrwv.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gcttsqwzo.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gjvhjwzur.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbejvyxre.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gquudczst.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gxoctchnt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/glkesvbvj.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwjvuhrh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrevlfrs.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyopkbit.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqzfbogo.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gacryqgyf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvbxucqj.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuiekxbp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gdxcxwqyb.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grftklesy.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkurmlzaw.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gutjeiuum.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gbpsnjfmq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/geumglvzj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgimgkef.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxrdlpszd.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gjynziwce.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhrswccc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gydvlbpmr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gquwriell.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigxqnolt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpueqduun.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzxxwfvv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gysbluzqs.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/grysygqfx.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnwzfojc.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpemnkdvs.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/goqsbdldh.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gylhhdnux.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxlxmxpi.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxclaevo.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/glpskmkkq.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/getikcjku.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gtsudjowk.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/glmiyocro.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gmilatwvp.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhjdnldm.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzndwdcz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjqllwbl.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gniqplbuf.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gnwqzgypn.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gplyqnnwa.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gnriacspc.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gduldjdmm.sHtML


<!-- 参考信息 -->