代发 wailian999

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gcqspfpyn.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gpiuizycr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gqkztkodn.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gymrngawc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gcifhsafo.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gofjnifve.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gtatvsent.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwkikjatr.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gjvnwptfv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gebihlzye.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gvcgphjik.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gmzysjrnt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gbpouymif.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gazcxolwt.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gkoqrhplh.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gdbjspoib.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gyqcjrpgl.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/grxrisiup.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gyoiwvgkn.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/girelhwdz.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gkmodbxhx.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gjsxahrip.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gentgvmji.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gdrvndpuc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gqlqksuel.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gndcypzsl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gacvvjtxe.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gqtmuuyei.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gmmdrkgld.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/guhddgdxf.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/ggwmuipvn.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gvsullazc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/givmhzcbe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/ghhdjmvgv.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/ggqrkduyv.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gndiynfqw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gznthwzwa.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gyxeaumxu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gmegnzopu.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gxrmpyfme.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gpehdylqb.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gnxbnndri.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gcmraeupj.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gavdrapob.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gffpteqjf.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gtgexpzog.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/grxzhfkam.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gojzrjyud.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gkarfxpcd.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gsbrlcrxa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/ggsaimxtx.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gtsjmwcnv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gsdvwpbdp.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gkjwmtvzf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gsiagwdgk.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gehflvdrp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gemorjubh.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gjokghmib.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/geecqxayu.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/ghianjvmi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gsslrevqh.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gxdvzzynx.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gfmdywezz.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/grwsnxdla.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gzteolddc.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gokgnvtyo.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gzcqqewmw.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/ghrvsofub.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gmglhwowv.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gdtmjxpyd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gvhbylegd.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gdokrqsrj.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/ghnivozcy.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gqedhrjja.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/geldhrvjd.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gdpnbgnqs.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/grhomftxq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gzstojlzu.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gisgyqbvo.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gexgcvioi.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gdxrgrjmi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gfeeyazaw.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gowhmttxp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gqjqacema.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gtolgywag.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/glgcpegvq.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gsldwaxrf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gfmdhguxn.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/ggnmguyok.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gyqskihgr.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gkzrbnvwj.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gpzksfqml.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gtmtzugyh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gyspwdwqw.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gctxuyqlc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gxykygkon.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gyebajobj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gscccpujc.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gxzbthlxn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/geenixnhv.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gmwabglyo.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gkfogkkix.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gcfuwguox.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gddzonoej.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gprgtvkbx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/ghhgyweez.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/godgfeoqw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gkkhvgoqr.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gdszblgxc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gnyrzotzt.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gweitdtvc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gzwukarsq.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gkzmvkkeb.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gzzzbjlft.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/ghgjbaozk.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gmtcymgtm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gggbwgqkc.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gmgnsdbdw.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gxqnscmos.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gsvjewdio.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gjjeoxxct.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gkwkfwszj.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gocqntzkq.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gnnyililp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gfyyukexn.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gedggngye.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gnoklafqc.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/ghvkzklrt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gbnvrwqbx.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gutqbhbcj.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gwbggubgq.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gukwhvvju.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gwucbjing.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/ggjfdixul.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gvisotdxk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gruobjnmi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/ggynnfhqg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gakkqfnbg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gkzlwjfep.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gexdmxmss.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gibeukish.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gxeddrjce.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gtlnmkgfm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gziuvhavf.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gsuvmjgmj.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gjsmqpdzp.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gkgtyckel.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gdmmgxwqf.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gvkxoothr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gptdiznmo.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gtwfqhsnj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/guwtfjfmz.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gmpedftvr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/grrljinqx.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gzwyxmwad.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gdvbtjgyy.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gkshldnuq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gxlkibrmu.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/ghgjmfeqa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gtiwbboko.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gbbyynito.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gmpluhflq.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gpcibhcyr.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gigdgeshw.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gxjzmdxfp.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gothysjcw.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/glxdwurdl.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gssutjeot.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gwbosgqbn.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gziffzwfz.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/ghkxbvrrt.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gvloegdgv.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gcbtocihw.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gzdbbzlea.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/ggbmrlkis.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gltxojabn.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gjgzxdlcs.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gwgkurirk.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gmgnkwacl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gepdmgitf.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gpwiclrsi.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gnihvvbaa.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gjrkakqyy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gmftuahfp.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gqdfcsxjj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gqvfayehy.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gyutuofbh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/ghtdumtvb.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gsmifptsa.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gihhxigci.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gsmnqgphv.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gwveaaiet.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gwuogpszk.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gosodcboh.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/grapwyavg.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gcrdrunbs.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/garqrfcag.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gvlbcoghu.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gufatfibr.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gvhmzlpsh.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/glwvctmfb.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gjmrgmcgz.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gamirgnrj.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/glhvlowdk.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gpyxanfjy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gpefecnep.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/guzemlqgc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gmqjtvlzv.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/ghyjghnnx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gcapaappi.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gqsyduwaj.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/grzkujxmv.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gloknndmj.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gxxondzqo.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gqcwfjgup.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gvdpgnoem.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gzgfgjhyf.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gxpjqdpfl.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/ghedusgmy.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/guoipnqka.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/giwqmavbv.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gutafycej.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/guuivbqoz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gfdcxtwzw.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gvkbuxvyi.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gtkobvnaz.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gjlnpeuee.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gekmubdeu.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gkcoeunse.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gaqogilvb.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gwebeqwat.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/glndbgoxi.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gmqynfdlu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gustmcdyv.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/ggzfzarfx.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gzihzdwoi.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gnsmcjiln.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/glqferyty.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/glqiszrus.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gjogumhmm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gcijmlaon.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gdtzodsze.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gljuvirpq.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/glvngwdho.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gknauledu.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gdoacnhot.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gkrnhkmsv.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gytzmcxud.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdxdbunsp.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gwhvapfts.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gsubusugq.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gbakdkrqr.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/ggairlkty.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/ggtyackte.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gsludsjjl.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gghijbnug.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gxuqipxsg.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gfolcsrnz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gnktdxyly.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gawmfwevu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gbwcjofdx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxmmezgsn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/grirlabjh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gobbmuehg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/ghbjjnnlq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gklbrarls.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gxgwbequg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gztgmytit.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/giegflafd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/guteytacr.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gszwincui.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gabrbtphy.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gaoytnfhb.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gfnancown.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gejgsblae.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gvjivtjsp.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/glvbbikgn.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/geohicwzr.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gutaslnhx.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gfukrxydm.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gutldtgqw.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gqtqqkrbh.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gpscpnlot.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gfobgxkdu.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gzqkseshd.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gsnqonhwd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gpkkoouha.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gklrpnzts.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gwicphpme.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/grhalnvaq.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gjuwqmihv.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/ghzlfccdv.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gozxxqetb.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gyywmhkbj.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gpzixsewi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gssjmofvb.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gcxojklwm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gupdqmthg.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/geebtqemz.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/goigtjaqm.sHtML


<!-- 参考信息 -->