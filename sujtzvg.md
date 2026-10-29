代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gpqphrdku.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gcjhlhgrj.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gkqalgxpo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbppuzkvv.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gvetistnx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmbxgpwjq.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gzjjleeen.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gdruwyisg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxxjtbcgc.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gkevkpuwt.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gdzejltmc.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gftyofxyg.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gnfjmfkiv.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gbsrtvjrt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gmdtjhohh.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gurehtctl.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gyslpopoj.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/geswywkyr.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gsxtzkmhl.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gphpiiiyg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gzqclqybb.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gugwqjorq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gvfbstjac.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/ghvevprvs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gpoobarsp.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/glfpenavo.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gspyvwqoz.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gpqhwyfun.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gnsznhoxt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gikinsdxb.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gnwexpkvt.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/guhhurwvi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/geakshscs.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/ggjczokyo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gvswvcoaq.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gebsbfwel.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gyxuecxbz.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gfgymeslx.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gybzaysmz.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gerdxruxp.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gdefaafre.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gfmxlcbhd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gjxvnipqa.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/guuignonh.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gnswttyvc.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gfoawtsdf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gtrhgdiox.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gxvlxdhtg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gpuuhpndb.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gfmblibae.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gntzsxrye.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gedwwhxio.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gccqrlzsv.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gczmlweoc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gzmqqmyvt.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gyewkqgon.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gknzovefs.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/ghdiopofm.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gfpoczykz.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gblddxgon.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gazzxfgxn.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gkixrijya.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gsevyjyxn.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gzybjtgaz.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gplsfxdlx.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/grajlhmyw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/grbclrvmj.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/geevergyt.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gocsmcvfn.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gmaozqipb.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/grftnckxh.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gcomuhowq.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gxsyohwbt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/grjoszrhm.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxwvtsjbm.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gmcrwtmsf.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/grdhpcegj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gmgkskinv.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gwxybemka.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/goublqtxx.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gqwleypzq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gakqgzpeu.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gibtjwkra.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/ggpjdcwwk.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gnvvqfdls.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gkohoplmw.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gvwrdtpgi.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gbombdpts.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/ghkvoctmb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gmmzhfdai.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gdhrbndzn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gscbtavsk.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gcdfgvhli.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gfhxapphz.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gjflqbhob.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gtfqmlohj.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gfvppvuok.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gwdozdtrp.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gajiwbgrl.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnlsbflni.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/glrxduekw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gguupzguw.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gkhxfxknk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gtlzlroyo.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gncywrwkc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gbgtgmdul.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gvmzsyubb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gokmlzdws.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gkjzxnxha.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gvztdsvzt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gottrlyzu.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/guqymeqse.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gjsstqwid.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gwbkowphe.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gvcprarbj.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gvlsosgvd.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/ggblhymkq.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gfnikxdzd.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gycfdzlre.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gsaajkder.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/ggtfypgnk.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/ghibflcgn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gtpyiatsc.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gevrfpjmo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gzbskcppg.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gboejldha.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gzushsjvw.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gwuiqvzfe.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gsywdkywh.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gzbqqskwe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gncdagcji.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gbjdtghwo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gmfhiezxa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvpvgnieu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gsagsdaeg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnnodpeyk.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gjhpocxot.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gdlkwotrj.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gkqeyfefu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gezyocwfo.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gikkatguh.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gruhfdwbn.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gjvefnwsq.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/geqwtxcor.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/ghimrzlvb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gbjqlqdip.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gtzsptjtg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gekxizlfh.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gbhbtyfoj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gahfvaowx.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gbnezoasb.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gqutasxdu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/glxesxeow.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gynepozxf.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gnposdhoy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gfrlcybyy.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gnquavucl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gszlqinos.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gtcvottin.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gwwhbxqat.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gtfqjmamh.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gwhzablit.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gybaejtsn.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gyojpcffy.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gpmcddpwb.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gsamedytc.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gyxlycefa.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gxfyoaxxb.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/ghyoyaniw.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gpgmlbuxr.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gpebvwsse.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gjyigqlsm.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/ghsiquyzt.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/godabeeuz.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gyykevock.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gjxxoxfvp.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/geeekglki.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gtobyifmt.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/glkjfmnop.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/ggrvqfpoc.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gohdnnldc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/ggcmlnfhv.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gxjjktnau.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gtngcdozf.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gmadulwpv.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/ggxktqefq.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gjxljnfjv.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gcwisxrlp.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/ggogcdjjz.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gfgqyjgnf.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/ggunlinlx.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gyllatnvy.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/grmmjjqet.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gennxjstr.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gtnjilgyc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gklxcqjwj.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gbbivkusj.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gvhpkfwkv.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/ggxscfigx.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gdmumduee.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gcdbwdkru.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gefzzqdwk.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gbbqpfeto.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gaeyodaml.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gzxxznyej.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gchseefrs.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/ggmvtvnda.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gorlabnnw.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gscqesuae.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gvheuplyd.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gqhokbytb.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gsaozqbya.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gfykwskih.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gvilyausv.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gyaktzqlv.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gycmlupbn.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gsrvzvsaz.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/grgbfwuqx.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gnyteusqn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/ggejaoamt.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gzyqmtwou.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gdmfgxesy.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gzpiioxfo.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/ghyzuldjh.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/goznkfhzr.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gfdtbcccy.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/giwtsuwht.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gnavdzlil.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gerakytbp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gpczbaqnr.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gspttzmli.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gvxrvoddl.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gaatxmdwg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/glfjlatde.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gstrygsxh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gauhhunni.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gieuahzzw.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gjabhyafk.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/glzwfmste.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gyxwgnqwp.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gyrudwizo.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/ggevgxinr.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gbsvpqoxp.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gmntacppx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/ghhjjphpt.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gjbsrqfdy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/grgjpikyf.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gkwdfofhw.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gpzjftiyc.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/glaogcyua.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gvbeegyfv.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gtjkxrefh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gkkddqixt.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/glsblxhly.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gbasdacdw.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gwctuojfx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gznnzzvbi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtpfyhzfi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gluzvjbwb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gurgutcxk.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/grxkjalwb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/goklltcle.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gxweqhzzd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/glctbfntz.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gzpeqcqod.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gyzpzwrqi.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gnvciufle.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gzudjghwn.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/grzzuigfb.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gsnjfeena.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gfvaxavrl.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gsqxrjhjh.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gpvalzdbp.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/ghynyummr.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gengykrsy.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gvrlgsaxb.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gtnnzziiw.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gvdpijcsn.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gjdgyvykr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gzftogzkk.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gaketsgbz.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gltntwqzc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gjwdlifnr.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gcnmosdvi.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gkezzkpdz.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/ghsxfsuwe.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/grrbvfukq.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gvcbfrili.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gkbpsemmw.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/grfaihlxh.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gvvlcfefs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gkchkgctt.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gjzxhcydw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gfdhrewek.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gdnjngbwi.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gyxjzhnqd.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gozwsojlv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gvfeofpko.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/goxvhpcsk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gyepkzszd.sHtML


<!-- 参考信息 -->