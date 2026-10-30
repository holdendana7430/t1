代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/galesqoje.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gltgwvvds.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gzufrsfhz.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhnlvmms.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gernrglxg.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gouiyxfgo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkurmqkbg.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gxftdevce.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhtbwbva.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gsxwbngut.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkgznddgk.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvvrygziq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxyhgxyu.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gomvvgilb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gldfwhxeg.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiuxxssn.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gjaaldpna.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/ggayyzvss.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjuazlry.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntuctdsg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gfweevflm.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gaulmykpj.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gecmocvnq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grnxcczzk.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpaxxhxt.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbxufzofw.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvcvxffw.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/grvlksrct.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcfgqafjl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/goekximac.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gzpgaihlq.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxkuslyd.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gosvmwyfd.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gbzfqfayk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gqhotfmjl.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gncwavhxg.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmojruaga.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gnevlysyv.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gcwzmorsy.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpuxkazu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnhhvxaz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfdcyqbo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gcdmjydes.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gyqbttqbv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gtukcjkvu.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwsejknd.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gcrmkrgnx.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grmbkgyjg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxqcelhu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gmnwsqcjz.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuvsyvfz.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyhpfpgm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesaggetc.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gwhoxhpsg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gzllzkwgp.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gukdcswuz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbizmvmw.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/givvqxmza.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gzisilbtl.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gqoafiosv.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gvkfjnepw.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/ghneoqguk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gyewkbaee.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gzyabgwve.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/grzsxclsm.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzossrwa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/ghwsaopfl.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gzqxxnncg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glytwevxv.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwzekpru.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxajynrp.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gbaftffws.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/glzdipyky.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqsyoxrp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxugartb.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gregmqrnj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gomagftfo.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/guwehflrf.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/ggvgiplpb.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexgzrkei.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsmxgpph.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gdxtyjacw.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvvmwybk.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwonwrkw.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gkyygqwol.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcgeieft.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gprxppwtz.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gsdbbfziy.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/geokvjgwf.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyvaupwk.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gliysigqe.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvovsfvks.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvimzhin.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggwvzzrlq.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnpfspkr.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gqnldgygj.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gecepulki.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gqfhlewco.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/goqtbdywh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfyfhwtn.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gobzqwoez.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/glzqlxlqj.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gurruurzf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbwmcuwt.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/ghogzsnfb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxvwmqgr.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuglpija.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goksieplk.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gasgucrpm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gvjwyjqvi.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gwqtouvya.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gghdymcrg.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/giyhqopyh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnypmnlaw.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcadylgwe.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganxyftwz.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqfmbiex.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyphyfks.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gnyjukbio.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gacxbkbfr.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gablmmgtw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnnkkpjx.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gsmretlfa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghhmhjueo.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ghgtllknv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guhntgqab.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goelobxvv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/guxlkccwf.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/grkdizflb.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghzopfjzl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdfuiihk.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gidimrlpe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevgmuwwu.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrylvbjb.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnygmdvj.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gnqhjgluq.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcetgmbmg.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiwxlgpz.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gpyfkeuuu.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/ggloryrjj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gxssnhxzw.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/guvbyvucy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/guoycyzym.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqwrasji.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/geaskpxry.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpufatpoy.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gmfxvtehv.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsagpydaw.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/guueufdlw.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkozwyeny.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcibuixt.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gmomzsjdw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gxbrsuwad.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtorrhihv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigmeewyc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gadhlcvdz.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlavagcv.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/glabblukc.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwihtuqiz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqgtnbzz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gszfbkopp.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gizszyhta.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxqmvrgm.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gtznajevc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwvmgyxf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gjcnwjtuc.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/grrnnqnak.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthbrxaxh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctcktfnr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmlzaevm.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfpcfmav.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavxvtzpr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswdyrrtt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfxuflwk.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gprkxdecl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/glsvemjpz.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gohtpgkee.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfaulrdi.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/ghjrjyqzl.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gglruhdla.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gianuemsg.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gcxrfphra.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gvetphfzw.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gotphsnur.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gzcfxnbbj.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gzjtqqrsy.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gduxmeiyq.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqywpfwf.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/grgnuprft.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgsejahk.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvecmxagf.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuztuybm.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gfilniplu.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhzwukeg.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gukciyomg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gqescyldc.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gjaihzesn.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyakpvoqp.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/glfofqqqd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gnpcopfpb.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkmhqfkn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkftltovn.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gynzvtjsx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/glsystprq.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gopipekpc.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntueuumj.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmvfqmez.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gfxwbpcrs.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/ggqiqdlup.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gvsztjsyc.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gvzjiiglv.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcpxblhb.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnljyikk.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gblfctlta.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuckdkaq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneaxbvoo.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfqbwkvh.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gaxteksno.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gktxxfxwh.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gymsngzzn.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctulhjld.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbguqyevq.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsypdgmc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpivzezt.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gvfkpigem.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gthgpyjyk.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghdeazzwu.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtncogsp.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gtvwfttec.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gklwvrxrw.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxauaznp.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gqgjuzame.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeqbowcr.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gjqvyqdcu.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxupakup.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gpyguwozd.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyckdfrm.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gaibijdtm.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gillxsqpi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/goukscnqr.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gewmawfpu.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gmtugzoca.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gtnrkatei.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplikjcob.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/goamgqiqr.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/getjhgcxn.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gitpimzvf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbwywigzb.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gygrvlfeh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gudmmuxjl.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gsjfhxebr.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgxzhaos.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpxbvzld.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqmdlfezt.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/glmnubrcv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxfxvxvf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghxpleltb.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ghkpmvjpo.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqismotci.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gneutadlc.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gcaopqkcd.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gscobusgr.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gijkqtdng.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gjljobyay.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gdwhlqopg.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gefbziplz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gfafmbkrg.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzpceqxh.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqbybsbz.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecttypzw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzmlwlmv.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/ggitoutip.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/ggkdmgxqw.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxabftec.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/giibhueek.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gqllwxrna.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gqcbkjfyw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grpnvsgrm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gyqlvpfvk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfbzldwi.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gwqdgqbta.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatizywil.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsuwljsx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvobampkc.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gebciksaq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gdwhtnpig.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gixwnznwa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcktxzffd.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gmbeqwbay.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxmrfobs.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gondzxjry.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gvgnjyupc.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/glxlytdjb.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gcsgcgsqi.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gvbysdtsx.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gxsslrpyt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnatwsig.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/glrjhsgpl.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gvrqjkije.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocmbpjnz.sHtML


<!-- 参考信息 -->