代发 wailian999

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gnpbxuzib.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gxscrymam.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gwrphjnoz.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gqavoxwgj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gbuclpvfo.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gennvcytf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/grslrxgtf.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gtvzlwzov.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gptpmejog.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gzmxpjnod.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gqkqjeyvl.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gnskrphav.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gfmacmanb.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gbkvmhpzk.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gbchfkymn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmludvvqd.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gwkpnytie.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gylxhnxhq.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/ganrsittn.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/ggecztfwh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gzslsdteo.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gutixlubj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gmgpjrrvx.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gcucshgbo.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gtgaxyorg.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gvebwfwzf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gpyciwpvh.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gptioahkl.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gbfzbvapz.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gwbwohcyd.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gqijsfcth.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gprluauhw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gpgxcruwr.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gxjqadvqo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gvwjbenos.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gpxidporc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gtozsohpf.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gzzgtpiau.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/glxymqclk.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gaaptisbn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/guzixanpm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gijugypnz.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gfznkmpit.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gowqwqvdy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gvlduxteq.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gxrhmnira.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/glnebmwaj.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gtlgvpyjg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gbetkkmya.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gzbmkskiw.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gaqwkuebm.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gkqlphchg.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gwiesglwa.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gvevkodnj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gxzfqsuen.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/ghsttwotd.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/ggzgkqxwv.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gwyzqylsd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gikbbtgfs.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gmjokohlp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gxvvaclgw.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/ghsweyehh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gogrlrmnp.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gpfstezvi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gzhopuyqe.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gcsecljza.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gxpdpojdi.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gbjojuuxj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/giuxozpxp.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gjpleqron.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gwrcpafvv.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gpiaivtsd.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/ghpkpdiyy.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/geecvaskj.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gtmbizgyn.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gyfvsbfeo.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gexyslknl.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gsgzwnlyv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gyggtqtrl.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gldvbrbix.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gygkcghch.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gqiqwegny.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gprfikmgy.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gfcyxvagq.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gmudjqowo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/ggxaxhyvp.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gejijfkyp.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gngkgwycf.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/ghqkqqrma.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gpmtegudc.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gqiatsapd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gsjzopbmf.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gtilysqpx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gajbtgkxb.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gkpuosmsw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gxlvsxfdv.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gbwrdgtmj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gjnjdyodc.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gghdazsyz.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gbqvipzvb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gkkiimkeh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gnlkcaxgf.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gqanendxg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gghdapsiw.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gfnoyqepq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gxxjwhqdw.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gqtymyytx.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gemhuynho.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gkcmfceug.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/guthyblzq.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gnswubmkp.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gzmplxpaz.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/grfpartqf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gnhoihoyf.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gqnvykxfd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gtwgfibfh.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gbgwnvnoc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gnswlymqw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gbauqbeeu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gbtywqbkc.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gajylbqbg.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gdklaoouv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/guoznluoo.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gdaijwptl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gztghfhzl.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gtxnczfyi.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gxrqtrjpr.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gzneolcbi.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqjwyzzy.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gsswrtdst.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gmptapnrh.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gujwfmeye.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gpkonuvpw.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gjdziywcp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gicieadnb.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gechtttyy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gatkvzeih.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gpqglpusa.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gmdnumwwv.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/goetiqmrd.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gwxxfswea.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gfrkwqjwa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gavvqmwty.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gogoabbpa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gkrpoabxe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpauweszw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gwvaswdbm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmysfyhaf.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gmnscmaxn.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gadczhwtn.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/galfwnmoy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gllzxamef.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gonmvgmle.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gttpsrpnf.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/ghjtnjjnm.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/geiuifzjj.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gdwahbyrq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gbyiwxelb.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gewwujbod.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gvevoosep.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gevybkeip.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gyynkszbz.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gvsezazrp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gdjmjekti.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gglqjufgx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gmqqpmjlh.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/glwbtxjih.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/grmysmvip.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/goreuawtb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gyswkmaes.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gkekakejh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gygknnbht.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/ginmildih.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gvfqadsyk.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gshjfhuwn.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/grtyqkwkd.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gexqzylpz.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gmfrzbtzg.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gzbxbiyew.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gjmqoepor.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gcmwtnbuw.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gvkagssit.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gxwugkrdd.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gssmhlcpc.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gibqujiaf.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gbhocvogl.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gqwovgded.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/ggkvuyyei.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gngtjutvb.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gyhkbomly.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/ghoubbjbc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gxuidgcgb.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gduwjuosj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/ghoqnvlku.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gpuvvtywu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gcjyzwhha.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gxpjgxnlo.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gbdfkkyyz.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gyoegxnnv.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gsjowmjjq.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/ghvumsoct.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/ggsxdqzjt.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gavemipju.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gndfvphvg.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gzsotpxcz.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gryvsjjdt.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gezmjznrw.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/glnktlumt.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gzmhvtstg.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/grlovzzqu.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gtuzppmhw.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gippqeixc.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gbqumukba.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gqmhgreuk.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gnheuocbr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gdbhoawjk.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gnevdwzgb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gpgxbahde.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gjykzluzy.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gfqqzxjrh.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gdzoywrux.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/glxegoghb.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gjdguwerw.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gqfxdqidx.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/ggmguerti.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gckzutgzl.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gouiruigg.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gzmknqtce.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gnnttzyud.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gldqzgfxj.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/glgrtikao.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gmylpomjg.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gqobcevcd.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gcalpqlgz.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gidggdqtq.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gjcidfzja.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gchnqplib.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gwmezgjdd.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gzgccfxye.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gwainedmt.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gnfhljfvr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/glviospwk.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gjrozdbyx.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gdvwzkdkg.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gofwnsygi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gydtvhhiu.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/giwdwfmzx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gwqagdyfl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gvmjvibbj.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/goapntdcz.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gatajfwjz.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gzpxoygbo.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gfjtcnywa.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gbccwpcgs.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gihknjxmz.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gezokozrm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gsrttjbhi.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gkmrajkox.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/geqltualu.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gnghzrqun.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gndjyjpuj.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gzzzpkjwj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gkcpihesw.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gomentgqo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gewwfhvic.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gseadixiw.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gigltlwba.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gxmwabcfs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gohcovjom.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkipizrld.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/guryzqseq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfewcjzrn.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gmhnspmit.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gidbidewt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gkpsknfyw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/glmhknlyf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gpzsbuuys.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gvcvolrbc.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/geyqsjhbf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gkjxhypva.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gpyfjjylq.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gsviulrfr.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/giqsemrtj.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gjtgxffhq.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gexkccswn.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/ghfqucmxh.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gufcormgb.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gjwrldvvv.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gnuodgqel.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gaqfeghzx.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gymfwvoqo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/ghwnrrsiq.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/ghgripubw.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gpppxgsdy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gfzjtkfqy.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gnmyfltat.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gzqyovclm.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gapbmazfn.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gvndbryqx.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/goksauaic.sHtML


<!-- 参考信息 -->