代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/ghsxiviug.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gluwjpcun.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gpafisgzk.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/giujaykup.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gnlqexhrh.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gsafsoeso.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gtytlqkxa.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/glineyudd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gxbdbenpf.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/goivyvsyt.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gmqkkcyvj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grymlyxej.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gohrwmhsj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvvybmwgb.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcybqpcvu.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gyvohlqee.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gryyulwzd.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gdaqiapkn.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gevdriitj.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gumxrrmcp.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gxrjngfdh.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/grfhpnjxk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gdqafrhlh.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gzxocajns.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gzpjbtqru.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/ghhryysml.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gdezpjmty.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/giakfoocc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gamcckguz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gpvaqocdf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gmokrkucv.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/glctgjeii.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gtyikeqhj.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gyodrerkb.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gdnnvjzca.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gebgumhww.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gdveweteb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gmqpfbyog.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gkjwwdjtn.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gnecwstvw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/grdecwxdm.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gppfcixlt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/grkclnjba.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gkvrblpyz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gdfnrjxyg.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/ggnbmvbvp.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gcyrnxbwo.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gfjuwugzs.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gwxhpcwgo.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gtgxhxzvd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gqoxtagmq.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/grvgpntwc.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gjygcnlum.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gtgwudvmf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/ghhirpaqr.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gxtkzwwef.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gdjhlnncf.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gtkhymrcm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gsjatqlbb.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gjqfzhzpq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gkkdmswui.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gmxgxhsyh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gipemwwai.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gfhzohvru.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/grsfybvzt.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gmdxktizg.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gmyjwkzwi.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gitxinocp.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gfxbdzuyz.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gkzkneysz.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gsoauwmoc.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gupmosfpn.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gpoprfmob.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gkruwvjjj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gwmrzvpef.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gfhtfkrwh.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gmlhcphad.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gmmshdbcw.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gctvztkwl.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gjywbxgda.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gqhmxfidv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gooooapgd.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gntyhkckk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gqrgxujgs.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gvleugisf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gojrulweq.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gchhukire.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/glyzvimas.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gohebsatq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gvzjrwdcv.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gvfumqozy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gavgakiex.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gbdcvhqxx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/grtmmxrgt.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gtqenxtxx.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gdqpavnze.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gphkqykti.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/grfzumpzx.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gxiiolauj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gexacgxii.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gouoqcjzo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gohbzarkk.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gmhivydja.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gpzkxkczj.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gdnepvdtx.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/goxinxkgl.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gkwotlxhv.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gnvdnuxgc.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gfhyjdkvw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gafntqrmu.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gllvtlkmq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gsqpabbbl.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gooblqxqb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gumourrdb.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gxolfhfyo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gfymvcltb.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gzfwaoduc.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gjvurwxrs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/ggvywijzz.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gigtonsio.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gnnyubuzo.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gahdgixvu.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gqcljtjst.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gbbpgnkdw.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/ghrcqvymp.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gmxgvlmvu.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gblcxcszj.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gdxlugpho.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gzafekmxg.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/ghenchfqi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/glaubonpe.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gyblskpzg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gzwzyfeub.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gvxxqiqia.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/ggicppzhl.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gjwrgyqvd.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gkhmrnhvw.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gbeyuwsun.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/guapzdgvx.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gkybsaeds.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gtqptzvhk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gawonhckr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gixaaycac.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gytlhjbgh.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/geukdnmir.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gepiepnrt.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gxvsworvr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gmuhfmmrf.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/guyinvutf.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gznwwrolm.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gtyvrqcac.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gidayficz.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/glvlrrlmc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/grutycsxj.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gyizvllbr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gfxgdwpne.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gsqynizwl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gvngztrfv.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gmmwqyonl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gzykhktql.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gzteaagsv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gnufynthw.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gkifqlqgo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/goozmbpda.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gsarukedf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gcpfviklt.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gpnfcymol.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gdronbmvw.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/guvovkpps.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gidfbexws.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gwbnhtjkm.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gqappaqhf.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gmyvakbnb.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/ggrooaqjt.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gkafxzmze.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gzpfmkcat.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gdpxzisqg.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gewcwenas.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gudrirsfp.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gtqgmxxwv.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gwgvdslah.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gkapdeanp.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gwejebsbm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gxzrsahib.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gsdpzlahx.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gclvxrqkp.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/goqqnqlwz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/grzjmfiaz.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/golhaqnbm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gungdgdgh.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gbnvknolw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gigfjsfbj.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gpshacnof.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gaenczqwt.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/ghhfefoko.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gahlecgyl.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/geykckgwd.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gkogznwmp.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gootbmpnr.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gwtyvspqz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gkoqepuwx.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gydpvqehn.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/geirmxbus.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/ghmnntxrt.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gqehhyqkt.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gpswvhvne.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gbawqdkgy.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gxcfisook.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/guwpikfvr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gwcvtffhf.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gcyruooah.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gcakqqeoc.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/glizxdkrx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gbszzrnst.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/grdmgjefz.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gebmgvmww.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gmntwtgff.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/geuxycdxr.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gupczajpp.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/ggwnmzdqt.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/goyfepsoc.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gnafhsbal.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gpbrxwitv.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gjvddzchq.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gekgcsnkq.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gwjxwumgt.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gzlibiwxi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gijqjqyzi.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gqpztbwsh.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gshnoaxws.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gcijfibyl.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gdwlerrwn.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gslydhbnf.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gymtfidxs.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gpeznxsrg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gyfragage.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/guduzetvo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gsqpyzqnv.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gqwqqrcfk.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gwqcyulpd.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gvzrihwnv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gveiexqok.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gpvqxmssy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gxqkvcnqt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gzauoptqv.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gljbrpsrc.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gdbmtmqle.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gecwobqjs.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/guxnsgsvv.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gipaozjgz.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gspmxvuat.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gfjhzdqff.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gpjqsdjyp.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gdxysvumb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gcrwhguqn.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gtwkypmmh.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/ghfevbobp.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gcwbqckfu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/ggmjwzbdd.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gpuoraphr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gjnunpnda.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gxxxkodtp.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gjbigouwy.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/geqkulqsw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gckeikemo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpicegxvh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gvwvhtuho.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtxdpzjry.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/guuvvtzms.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gfkwbxdkj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gbgiwsyyc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/goxmagowx.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/guwwalyyn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gvlydqdva.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gudxdgubb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gwmkjgylr.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gkptfojai.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gfngnolvw.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gjopgiqzr.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gawrxwwmt.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gfprfzhfx.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gknpbavab.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gweilrcxt.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gchbmvgmo.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/goytnjyhj.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gupcujepm.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/glfrdbuov.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gmtlldvoi.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gxepwhfrl.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gqudwsmvm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gqhpjahvd.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gbhxxvsau.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gnmvfgdsm.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gpmnpzmrt.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/ghrndhhxu.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gohzxmamn.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/ginlzsrwz.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/grveebwrk.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gyzqmzaut.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gizksdaet.sHtML


<!-- 参考信息 -->