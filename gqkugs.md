代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3qqvkcwwm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3nygvvzrf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3fcmcjemk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxycaivg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ddkbyvoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3otgogenx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tqaikulv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3gxwlhsqi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqbypmdr.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3gummawgd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3cxtuncqw.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3btsnbffx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3pqdlscyx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3axzmsngs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lqpntdou.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qdyywwlr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dhdbbcbi.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ngarxbyf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3drbryxaj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3hgbjrsju.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3mmfgshsp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3elqscmhv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ivbozyid.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3xlprfove.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3agxowlrr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3hmrrmmif.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3urbkpiso.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ncrlbojn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ghfmemge.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qcahgfwi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mbfuuegg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3olyxqypj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vdnypyvz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3rjwexirs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3yeuvanmp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3mbixwuks.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ukbmzhox.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3assmqeoj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wjcagyfk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3jpldiumv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3yiqoqoxl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hlkkiupp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3utaroszj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ifbivaah.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vxknkbut.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3lwvjjycd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ilshdzdb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3figdegqy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dvwiemwy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3fnaknrge.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3fnmlxwoi.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3gvapvpmc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3dalodxnk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fhbxnfwo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3lotlckvj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3jcyvwbwv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3kvssyaju.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jvsvaftv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3rreghhmt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3mheqlkqg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3pgwwpxvx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ruhavvzn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eufwtqzo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3xqzhbpjb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3snferjbt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3gdxvobjn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3nlidbdig.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3jlempimn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ofycczdo.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3kcphaaye.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hfnogezc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wruipohr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3vnctndml.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3fahnalop.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jtipngaa.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3khlwcjam.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3stwvcqch.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3rtlpupnl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3logpdxcf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhzmizbq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3upkfzpzp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3inwyddss.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3xuyozeis.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xivyvqgu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xalkzbwt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qxbprkgq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zwerchbs.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ybbiziny.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3muoatpbo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3bgonbzld.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3kpxupkyr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cfpkwsyd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xsouzfrf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3rygnoaru.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3uwwbpiup.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ppeyshdb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3wnqcmmkq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ksnbrfem.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3kpunzcbu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3rqhaffqp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3pvdfbmoz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3yqexgkpd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3gwebtpab.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoervncv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3erwfpfbr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcpppran.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kxvchnev.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3utiuzyvo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cahyjhey.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3dlquuyae.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3evrzykba.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ufmsfdsj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qqvbjrrg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mozlxnhb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3xsqflcix.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3plfybgbr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqjqlbnk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3osdldacu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3berrynqd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ozukfnop.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3dshyjplq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3uoppfbxu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xdbxfnhu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3vvpvvzcz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3xllvjovn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3klzeoeyl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3exyiztcf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3nhrksqmx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kqwjoieo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3wdsahgjd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3kjgyrbxu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qsvrthnk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nqlaqlmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zugzdtmt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tjyfclij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbeaialm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pteteiwk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3byeknwys.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3oohkpypd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3noejvvre.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3snjbgntx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3itfhfwet.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3clgmfmkq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3hzzjomgm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tvmyruyk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3sixxppyp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ubqxqrxn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xbfvvbel.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3asopttqr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3satyoior.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ribvjrsq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ejjidgux.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3cgzsomdb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3oxkfuyrg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qsmqluow.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3yrgrhrlk.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ywhgkwnb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3lzgdcskm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3pykjdouq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ruresoey.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ggwrvegf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3likrkqys.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3cetmnlek.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3maudeiul.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zghfbsmr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3pfbjxawj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yxdadirw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3afbaihqc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3pcrjivyt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3einarefi.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rilwslvo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3arlzkjan.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hargsqjm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3umhbcvil.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3obnswplq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kicfldyz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uapxisqs.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3qvhravao.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3eqzrztuu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dvmxnqwp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3lowbxxyf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3cidlbdqz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rueibvsq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jaiojztf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3qlvsjywu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3fvloehpq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ddqzoefa.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nzqndyky.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3shatcncp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ojjqeawq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bufeuvis.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3goywmbsd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3poygwnnd.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3rnxrbliv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3jwikkmqa.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dulwfzql.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3huagvzli.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hwwgqgby.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3zktkhvgx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ovxabbrp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ymjlpsti.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3jtgpekwp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fkshxuln.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3wzbwsdfg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ehpdqowk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3sbwjxkxi.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3yahhkymr.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xcmptemy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tncqcagw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jmoalrpp.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ywvslxvy.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3nprookpk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hndpwopv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ylxojieu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3luvdqyej.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3omqgoemr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xivndrwt.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jmgcwypz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ylueuqcb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dylsgseg.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lbxtsoxb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3cyxifoxv.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hpbnniec.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3rfjxizwe.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3isadbhbe.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3pemwngbf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3zlufrnry.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3swyzetey.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3naqizuew.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3vbvqgyxq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zixcpjay.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3kylyirzt.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ylwajexr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gcjuyccv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vnvmrtrl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3qvfujpmr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3oelddbjh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gkklhblj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3plsdmjya.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3qwgceuio.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3qsuwsget.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3onsmaxio.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pyouzhll.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gttaqfip.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3omvhhcxu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3iafqhozy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bnmosqzr.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3yofcgglv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ltgksois.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3urrvztzm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3sxjehsnb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3eskeczer.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3bytzrcnj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3loojgvob.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3krvthrbp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3fgllwmeq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xbsucywe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3purnuyee.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xobnziwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wtjuqtti.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ikfsbwvq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3mxpsfamp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ixbicimm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3fuvrvlfh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3kkzzppjw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3iolmkxhl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3gtmfoqny.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3xpioovzw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3esfzufaf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nxanvzvx.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3lccnmxhq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3gapdzmqn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3kujkmlpm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3icwvgnpl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3yillzazz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3qooepsdr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3fdpazoip.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3thxkqsda.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3bkseneyy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3nxltjnem.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3fcynwpow.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3xmpjdqoc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3khgupmtf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3zyrwqefh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3sfmpnnrb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3koasqtio.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ugnygdqw.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3uqopojre.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3adxhmikz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ywdfzosz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3forvynzi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3dsezlpgg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3bhmurepq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3brdlohkc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3zahntpdj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3cnzfkncm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3hbxgjmir.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3wltfaaer.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3lwhmmhwx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3mqfnaibg.html


<!-- 参考信息 -->