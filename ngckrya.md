代发 wailian999

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghynywnav.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gazgosqig.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gopoaoyzc.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gibrisgjn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gaiohzgbr.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gddtcfxwj.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpojuypf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagkcdufv.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmtsrmyv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvssvczc.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gmflqhouj.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwuncdoq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gocztptvq.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgccdqxd.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gyjbhkuxu.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbreyjbrx.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsjjyrjy.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gdnrsgpcq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gsmipifzj.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gkratzdqu.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gyomasdzj.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gykhiwwmd.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoqezpew.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gwuelwnfo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzlguwgl.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gosnwsrsi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvypkpmqz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyameymd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gfcisbbsc.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gqiztporw.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gqznekmly.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzbglzqqa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gafneamfo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gpnfhvigk.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gmoneaxyl.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqdesbryu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gymuhauuu.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gkekxfosd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gunpnybln.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gcegsemoo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewvyfjui.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gxqelrtim.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gkpvsfpfu.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gesqzuqex.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvisujaha.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gaukpmstc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gdcbjsveh.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvytqsomn.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gtdhicvmx.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidaoxwez.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcrjdqiv.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gynykudbc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxnaimcr.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gykabwthl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guinwegmh.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gnyzgnxvs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gegcafutq.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdcsmcxh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gosugvzuc.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqecsvepz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwrnzala.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjdyhwue.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijsrbexd.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfhcmixc.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcjammci.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gcbdwfunp.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gphgnoftb.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gmoxctecj.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gsldnspyt.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbeaphrgd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbahjfckw.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gnzxhnfzh.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/godeuggcd.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gmewfglwt.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwccrppj.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gzqiatwea.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gwawnijme.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrktvixz.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/glirlgzrp.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gozutqtfs.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/geyolmelj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gutpklbph.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvjhrmkc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcguhgxwy.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gkhfuuhcs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gtpercnpf.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzrguzsz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkxfsmdx.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/glifutqdo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtmkyaxj.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfxixjzkh.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/golvbxbly.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gaaciqgrc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/goosgwril.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gssqssmat.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtjrkdsn.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuixqnbp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gacqrgstl.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gktwbhibi.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gpnnknryg.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvjzxkah.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoxrxkxm.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchegzgqj.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzdfbokdh.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubohvbyp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gixgwamgb.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gprtuawzc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvixpvpjp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gailnnrqn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gptragkjr.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdddobzhk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhfciboi.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcobfkbxg.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdasmwlpx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gcztmtfom.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbnogztt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/grjlldrzd.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyujculdn.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbwejgts.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gdwuxwepd.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gavdcayjj.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnfkrcko.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gutpsvory.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gusuqykmy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjslkgnin.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gtgorxxre.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/goyucfjyn.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gikjpycyu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxnhppxlm.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gtbxtbsti.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnonlygi.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/ghkbpboxg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkymlnixc.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuodjozh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiyizsuj.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gydnmtsfg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyjvigdq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/geqnulucx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjuuhwye.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gimuwbnaq.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/glvcwhpdv.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gknahxxph.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvpqkjnw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfelhzmjv.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gnqohzijo.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gwcalghcq.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gklwwxbpe.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gjkhdzqsu.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gqhdkrgsb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gykqmyugf.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gnlxtidvn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gdfabbrcb.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsyhlfpa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuieytwq.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgxbagsc.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkddkibhh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclehnzou.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gikicmlwh.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucvqumri.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gvhjhfjyj.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gfruinkex.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpujsdiv.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/glqirmfte.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfkgwsyn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcehrbte.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoxhcfct.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgouebrc.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gaomdvgmv.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gwabaalas.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gexrjwhtq.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgnbslsd.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlscjycm.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gciuemwgp.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gebtdpjiz.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyilgvuq.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/ghavmpdut.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbefktxa.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcngkvhjd.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gddptksgx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gayvgsymd.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gaqidhyfr.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gjkjxgdvg.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gttoowojk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gupjcuiku.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfjnjoph.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfooshdpe.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/giymeigzo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gyxxncidf.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/glpzfutvv.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxguapoqt.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gzgzdlpxo.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gnehxwtka.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssvxjhfs.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryimyual.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gswclgmpa.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gpahgrxfj.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gslfdzxuf.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklsykohr.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gycerqdhe.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlhonwyd.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvzgulzy.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gpgegxssa.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggjazfzv.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkbbsnad.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevcphxct.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gpxrxwuxs.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/goiyulqkj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/geffwhllz.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuhngbjp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gzcegyrlo.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxcwluot.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcnpkowi.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtywmxgx.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjtuldja.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gnqhcowzh.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gtiqvogss.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/grftlirea.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gidpmjvlm.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gavheixhw.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gvujniqta.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtfbucbw.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/giedrthgb.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gttjdaotp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gxumpmgkg.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhbakgdo.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyqolssk.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gfyryjhqe.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbadlgceb.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gdmhgriqy.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gskjorpjs.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/ghouzeyas.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gscyhdgrx.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwscycszb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwxrtjbmq.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfkchiqq.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkwmxyiw.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gibwlvuhl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcxrfrcph.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ganfopmwv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsrcsoyo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfmermzp.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ghzsuxuph.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqovlsglp.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlnyngun.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvuygizb.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gvamemhsx.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlshqvzq.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gsqzditya.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiamthok.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gtulwazpl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsysynfzk.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gtfywpehm.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsagcrlws.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gpzfsxfcx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gdjvakaoz.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gdbqalxtt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gyjmrfpgm.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gynqmpjlz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbhzswkq.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gcsgtbpkw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gibpfaepl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glptjthuj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghajxcnwo.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtynjkbds.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcokconyx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyeuqbfl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/glhkqdpsf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glofmizkt.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gkctroeug.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gozpkerzc.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gojwgtwkm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaclzags.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyuqkddo.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvxsyust.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvezamue.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gmwpbuvns.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gpfqmopvr.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbklaxkm.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gybxilmch.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gpcehkkaa.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/grbljivgx.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/ghbyqqkuq.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/glahmqkry.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gsawhdtwp.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gjjameykc.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gamehggoj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gzidksfyh.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gozihwfqk.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoxsjenb.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbziljxo.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gpbzghkfs.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gvrhugagq.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gjwzmknnt.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqweoobvi.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gwelormkp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gyrgpuytc.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbhyoccz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfxaujub.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/grmyyollx.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gftppuexy.sHtML


<!-- 参考信息 -->