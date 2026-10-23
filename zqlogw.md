代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3wmluksug.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vnpbozuq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3tyemumrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3leqlflwo.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3meouyxvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aemjwnwn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qwasrxjp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3aemahohy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3jzpjodjf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3knqxjger.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xkzxtohg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3cayebtzu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3bohlypik.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3npocrzam.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3serglknh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kktsluoq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3gywptkuk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jpikucpj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3karfzvsu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3gfpzjbuh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3bdychikc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3vziukjuu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3itqzupal.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3wqtjjvmh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3mvowirjd.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vweoxbxw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3khiddeqr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ydsbaaib.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3mcuzgndd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ltryihny.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ydzarcye.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ymivhrhs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qjbgvnif.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3wldywejc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ginxorsd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cfvzhuwy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3kdblqzar.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3uutzkqaq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3stlfjgjf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hemrypdf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3cosxojca.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vgnoroah.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ukviwvra.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hutznfas.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3assviynx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3rkjmfowf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3swaobvmx.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3llzfhwdm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zqrnlsoa.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3jthxguox.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3exuejskx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3fruheftq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3fkfkijwi.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3neorlrbe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dgwxywto.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3bkbycibj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3fifukvgt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3tnywtiaa.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3abrumnsf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3iufcocjk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3xqyaqqlc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ulcbjwvk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jdvnfpfm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3xnocpoux.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3scflfjzz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3zzrabusv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3vnrxnyps.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hkgvagcx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ixbekwfw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vqcpamps.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3shnrvjuy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rxwfjazb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3vwfrxphb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3epgmrvrd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xdjcyrtg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3pkaygpag.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3rnwklwnq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3kicykfoo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3rhnjwemo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3zcqccegl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jikpgmsp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3aoszwzqv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3dqiixdfq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sslatjwu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3dldctkyc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mgshqlnv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3jfenwjal.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ldtorlpb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ahielzta.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3marxhvoz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3nrwojtaa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wngvqlkk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3sojbkqtp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ripylctv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3vumplukg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3stjqoucb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3tabyuwnv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tfoclcbh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3otzbnoop.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzfrtoqj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3agussyfi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3csalyyvp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ufaqmeff.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vloiojte.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oymyqcof.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wxabuynm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fqfbohip.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3dxndhaeu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dqiqhwoy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3cmcqzuzp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jpvrboen.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3idiqpzhz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hfbtaezu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qxbvsahr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3gducejrz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3oyebamur.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3uicydzzv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fpulftpm.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3xlvhrxpe.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3wwwnxlpr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sfxqswgo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ykzdcmkj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3dthydobg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3cjtthfre.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3acmzdxyu.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3odvcwnqe.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tjfoivoq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3vgkxrcbd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vrpcuxko.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3qfxsqimc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3anzyofev.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3mrpveboq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lrinxhxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pczlmroo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vtemkdrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vohqzohl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ixwxqhye.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ubhaggmt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3hgujzrgs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3efckaebj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vyrwhpvn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mwmzbgcn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3pbgqmqlp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3mbbioqyj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ciismkls.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3pftsqeqj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dklsmdxb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hchsbwdw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dehmzaig.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3gmexmmfl.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lfbwhngj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3yetwcsvj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3kcvkojju.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3hdoqdbtx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3jepqxztl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3oznpdkui.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3jwmszpls.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3viaewadp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3adihdrxo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ndksmifm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3awyznouh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3pyuokwgk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3unnbakrk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3asfovlby.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3fxxtzdfn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kqfvngnw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ridklbkn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xkjygfoa.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3wlgbphco.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3oqkhzpgo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hnwmhtvt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3msrfyqnj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3oiowtijf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3cwxlodfr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3nrkzyzrb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3szdxdryv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wgflbroz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3uqcksxqq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3hoinskbl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gunlojwg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bqtmkxtf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mlwjxkix.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3wcednryf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rivkrirz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3foqpmmdl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3gwzzpfqs.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3mrsjmyij.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xcnazhyy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3pvicxndg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3avjwuwre.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3iyhsxtme.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3aezpgotw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xzowknqp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3edjustry.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3jguvhvmf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3xzykhstr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hmkkywfh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3phajckyr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ahzsfyfj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3zjczbagj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vzimzbaa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fjnwljey.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3mevcpihc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3hhigyasw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3utxtplsp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3miakobjx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3lzfbkyne.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3yflrmkjt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ocguwnzc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3promemls.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ezsfbopi.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3mowinpst.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pbcuwyde.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3prcywmwb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3nnvllsdj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3nwzqftfu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3buvtpmex.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rjwpirda.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ekxkpfir.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3nfsqgdku.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nqhdzlpt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3byesfcxt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kdiasibj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmuhmjcr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3htvvsgpt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3blpszzwc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ipjhmfqd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3gacladzf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ofofrejt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3iduejsvs.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kwzokxqy.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3grevrzqo.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3urzbqrkw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3buqvcktr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ahgzkdpv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3qfixsvyn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3kztheboc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gdfyfric.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ivicbvlx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lhnbrjyc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3vnwbiuml.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iymhcmdz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kjkobwhf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qwzqdncr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3zfxxdfvt.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ldypdlcn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3uqrrjqlm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3esmpbccm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3onjbevrj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zkuwtumg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3urcojffi.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3lwztmsao.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3lvrwkyyq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3czcgbmnm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zlbeqbgx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3eaclzxmq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xuthpllk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlyvydfr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3sdjsuygp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfwmqebi.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3lcbnmidv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3swpgfwhl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3wyoiiyju.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ajdbmfwu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3drxurbfm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3bzrivzhq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3cfdyflaq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3hkmgbcsf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ggteolhx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3plabzhbh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3iurmqsfu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3pbnpwxdx.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3wbsikttv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3qnivjddz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3bxwstnzj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3rwbpiknh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3atzsmlna.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3rbsgmhsc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3rfbpykdv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3wupwcnly.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3xldnuanw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3cmvwkcsf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3hybgviry.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3deubyfwg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3eafadaew.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3zluprjna.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3wwlyeirs.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3kyjbghkp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3hccciahw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3indklgce.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3evasyjir.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ljrbszyh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3oxcnvcqg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3sboczumr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3pkdwmmgq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3uazrexct.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3fxgubdxd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3darsctzz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ftamycih.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ubtzqxnl.html


<!-- 参考信息 -->