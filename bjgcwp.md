代发 wailian999

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3rxpfyfxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xvkccvdu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aexngqse.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3aupzkfyx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3mslomipk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vpibkird.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xshuozqn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3vktudxan.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jftndiuy.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3kknsgoho.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lrdinbcc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kajnvwaq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvhweixj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3skwtrpdg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3dyovjzod.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rvxsosbq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qploocdn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ctwcahwp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3mcnlowub.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3moezilul.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3mwkpnyhb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3aobwimfv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ccmvpdpp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3asmohjaf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3dndkuewp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3twzhakrx.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3solxwtkg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3btezdrsh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nplplcjy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3kyzdsmnt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3uhxohzwl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qolxjota.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ciujzekc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gxmedefl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3qixxujrh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3wvajslee.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3oavrkjcy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wnpvelok.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rapmvwjm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3plkseoof.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3saizshbr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3egjorkjr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dfmavsou.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3eurvaqkt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ltbznuqr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3cjsfereg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3uanihtuh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vfiaasss.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3xlqczoac.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fogmdjip.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vkfstppi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3iwpupmbd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3xoidhhmk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dyyqzfgk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zdyvtcri.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ymntctcx.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mgubdxmj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3yqkgxlcq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uvnivhhv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3asrpidqc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3cchqoiky.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3doqyuocb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3iltitgle.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3iqnubxld.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ctdfxrvp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ingokhrc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3iavtolio.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cganmeks.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3pkxpteeo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqvbnpxb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3blujfjuu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vlltieaq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3auzwazko.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3utlvqsbd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ksdbpcrf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3tmdnpgfs.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3nmmxqwnx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oiawfuvz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3kqyhkitr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3szdtahll.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3fegvrehf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qaepobsb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3kkjpnogb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qehjzpqc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3pbfnktmx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3voshuuzc.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3thtajboi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3visysjux.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3tnzywoty.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3rwumrjlo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3txoqhlez.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3xwimyiqm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3lwxvffyz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gowdisec.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3nqjqolqp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3oqpdwsgx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3edbvzfoy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jrhpbmui.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3rxhzsipe.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3krnywexm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3nvmramyt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3uyeknrsa.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jdqfsruy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3tkzjznus.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vyttmuyc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3remnjbkr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mkukcshv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3lqvjvwzg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zxgaqqgd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3rpekhzkk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3vdsobqyt.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ayliohyn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtmicojs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3bfgvgnoj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ddzekyaf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3fiacvfdn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vtcdivnk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3nvtiyuxd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mcxbsszb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3bfhgnjfh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3uonauldj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ecncyitf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tuznkevj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3yzjfuxhh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3akrpdayd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3smenljmg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3chyphyve.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3arpxtosl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ottqxtya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbkjtskc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zgvaqmij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xorwezyk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3prrnrubr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fiftcwwb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3voyrjxbn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ubpsomza.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3satrvfgb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rxnfdspf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3yzpkccul.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3rsncfvbw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3yjwflzhb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3sfiflwyb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wrnchpzi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qaliyiwh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3joyynfyv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cmfyomwv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qdgrurrm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wklkadgc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3jskmdvtb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3fcrgfxoc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jwmjjxiq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3dluophmg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3tfjkbjdt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3moesfwbd.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3dwmcrxqh.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sqwvrunu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zhwfnrif.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3yobvrcpd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3cyrjijbp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bwcdlmjr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ufpetnna.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3igpdqjeh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iontlaxm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3szbipshs.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ofodbfsg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jthgpzxu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ywjcbzqe.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3nkpcupji.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ddcxjvmi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3zfkqkolu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3vamvpsyp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3uvpbsfiu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3gvyhpzxj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3vhsfscqw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3lcjifveb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3cxyklkld.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tbjtphvb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lvzwtrmy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3dtzcnhwk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bzoilwzl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3rhvgtlkk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3gvmhwgrv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3dabptvsj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rwdjlkpd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3knbeqkji.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3jaaxqyqz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3hubstlht.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3rwojzecm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3uzjsitxj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3sejtikcl.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3qzicarzu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vhhcuikn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3epdudxhu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jquvnqqs.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jioerhfp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3qudhkhhy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rkkrvdsr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3yhtvvwsm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3giewysqq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3okecorik.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3exffktkv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3aviqsybh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nedsbauz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3rlbvddai.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hmscqkji.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3imqxbxkx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3xhcwbokv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rtturhbt.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3avxugruz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eoqbqopx.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3yjgpoptt.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3oeynwqop.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gurzwbnq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3obnucqjo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hzuurtct.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3xlyovxfw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jnnbsczn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xkzyrsda.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ezuartop.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3onzxtbwd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3arbkxpii.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahhebbtx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3osfwhepr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofmkqtsd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3lcovtvlm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fecnchbz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3tsalknvo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3uwgdfpfe.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tsvwartj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vgmtamwq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3iokemphn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3jxsvhpxk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsoxprza.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wsskqxjs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tvdaclui.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ykgzyiee.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bmqneaic.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3oiqinaie.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lrsjkqok.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pdknmmly.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jdidvxyd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xwgoxesg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ukpbvolu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3kgschxcb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fsziuvij.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3emgpdvdu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mimtxmoi.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3fafzbuwn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rdkvpbgj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3chhfhazg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hwxwpfqf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3xgqqikzc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3jvwfhkqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zcsuvkhc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jsqgqixc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3grpgksii.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3aoocmypx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ykfshqni.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3pnztldgc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3egwirvlj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ypxregrz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3wcirfled.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wrabynay.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ssrzlexw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3fofczhfk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wytahhaf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3fryjthut.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3nxkaifyj.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3vtgvtfsr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3waydwxfp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ujdkxlcv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3etzhdoyh.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3yudnnvqx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3yywyciws.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3trjqdxss.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3wkkfxikh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3pmvitjzf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3iotkagzs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3adhnybjf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3tasxfxdo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3defblcxj.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3rnupmhkk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3hpyulsir.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3skbpaymw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3akfoqjig.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ekujcykq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ulwxowqb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3fqwerddl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3fyermuvf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3afawiyex.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3dmryxwej.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3lcpjknmk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3eprrvpym.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3yvehgqgk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3xfsiuebc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ojitubfx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qoikjfls.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ruuzhebu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3slsfcwit.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3btzohwnk.html


<!-- 参考信息 -->