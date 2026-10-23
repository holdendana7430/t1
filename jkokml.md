代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qfbghfgt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3bbedxuco.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3gseauqel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3seczufxf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3puilhgpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnltortl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wxzcxzpc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3vjgygfgq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3gujbldsd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3iuqttnxp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3rfpjqtpt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3afmtdpan.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3vehdeeql.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3mgnriftc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3clascjdn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qwrarkmr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3iymciken.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nsorkhnw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ewhoerct.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3mhrbsywa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3swraaqqz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ecutcqak.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3hgrpthhu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3rgelwxav.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vnptodta.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3eeadbsgn.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3bruxctce.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3snjehrnn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3naamlalu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gbjieecy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vgligtuq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fbqoeluv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wvnfrjgo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3nnhvahiz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3mptbnzmh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3aokjwzys.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rzlrpjfl.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3viveqvzk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3abyxabzh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3taipgnsl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3rxuseamb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sdkbbcpw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ltdyikrl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wjiwauer.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3eseppppx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3rcrvvbqy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gjkzbplk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3mjrnqdzh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3msqpmedn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3yvicvkqm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3xadiqwpi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gumlzawb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3gfrnpvli.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3mvkfmikx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xoktivev.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3qrhvvwwg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3zfypesls.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3fuqzpkiu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3solpnudf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3vksebqaj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3pfbqqovj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3dsfvbbkb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3agjbfmni.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3spxtquoi.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3womohdxu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3gqimmokc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3euxcsbbx.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3nvwrrxno.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3opwwsdny.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3jugfxbbz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3yzqxcajj.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3koqaygqk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3okyhqzrm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhvrskcd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rjjbyysu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ytrrawsz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xgdtztmk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3flteqszk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ejhruwof.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnmmgmkc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3idommofu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kkcvfiyh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3lwajkgkb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yyrzxhww.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3samanojz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3vxdxqfrd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3jdsyucrp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dijelodq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3hawhatff.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3mlfdspdu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3pdhrlcsf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3mmyiokqz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xtmhccqw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3febjhnyi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3sdreenbz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3evasvfac.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3eoktstkf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3syfoeqbq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3iycwqeyw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3olrkuuer.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3qrulabep.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3oqqrcssc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3vvvwjgpb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3bkmogecu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3tiypaqvh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hbfapuwh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ulocryfh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3kimdpjmp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3spgnhojw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rurjhinh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dxplnzls.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3bynbotgc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3glrfrycz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fwfvgbss.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3aqctguon.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3usqolonx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3gcbrtcor.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3gzprgwtg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3yiimvteq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3vzmvsfur.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3kfmjhlsn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3fkucifpm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ywffltgz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3fyhzrpff.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsnkmonn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3jjrxgjci.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3lushgtmb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3dpawnwgn.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3gjealwcc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3kcnynnxa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3sogikukq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3coejjiol.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yakyeulf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3miswgrar.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3lhumbyrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgfkwvha.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jscblxxt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pclnmsmn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rsnecwww.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3kyyuhlfs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ollgwcyz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3msfganmk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3exqpxrdv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jhdhella.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nbgasrwj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3yzihogll.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3azdcgywh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wuksncfr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3aowsttcr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3oghhlcpx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hyfscgbh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qwjyibfl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3xrcqdrcy.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ffxmjwnw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xuuuucxm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3mwwrbuyj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3zllpeeqr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3fkgiskar.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3yulgcatz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zwaqnbkv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qjnzkdoh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3vdebfovy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lfroesan.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nizqgyqc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3nmunimws.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3uneshmpv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ixovacgj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dmlegppk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qsgjzeaw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3aprqtpdx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3toktxlpm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3egpytouj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nuvpekwe.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hvvpgbps.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3siwttyhf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fioursmz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3czkoxvet.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3oryfjzvq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3exbkhmux.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3eleoluji.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3zovahyyc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3uelvzjfx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zzgdnqii.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ncgopuzo.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3jxetqpww.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3kwjspahm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3mfkvpibi.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3wjcfcbzq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3pcogmztg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3xlxqdgog.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ohaclyll.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3iuxelhfg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3wqrvuzlj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bxnggrzf.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zaivhfat.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3wdqxoser.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3raarxbfo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xpvbbmat.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3kwvtoiye.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3oekwzysa.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3laygfyek.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3urslwjbp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3jwgyzugk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3krekfxuf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3gqciqrgk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3fnxlrecy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3fzhxtbau.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3xjsbhraz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3plbyamny.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3zacxfere.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ttpaioae.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3eetwvaut.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3srjhnfeo.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bfeshanp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3awwujrov.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3tkxkaruj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ytmdyxpg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3feeigvck.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3fremlqck.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3nrlieyee.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cmqkvils.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ceswdqyl.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qtbnvzub.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3exkchljn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3aodsszeh.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdcfridm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3tlcdjbbx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3dmoumwfk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3xtefshiw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrallrdf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3mebbyphk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3gaysrkra.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3huslxmzl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhgchxhl.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dujxhkrj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3hsfxfvke.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3woidqvxm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gcmvypqc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3znwbyyae.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jyxholza.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3lmluozdx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zfwivgcb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fhcfllio.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3loqvzqwi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3amqzayhy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wlsplipr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lctpqkmf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3eazgzfxg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3klfmzwst.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bwrcysfg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3gftnfurg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3hhnwgqiu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3kesbvgqe.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cbhnhijk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kewetite.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3hqxojbir.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3pycwobxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpzjembo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bgrihjmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgmntvgx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3fjiuthhn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3jlvqvdyt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3mnetqqiu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3qejehfpa.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3snoxyuuz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3mdliavzz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3qqpexhja.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3vujfzdck.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ygiemcwr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ywqyipma.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3fssnzexz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3axvljyap.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3xrgjbypg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3djwgidus.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3rnkwrxvq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3dugjvzby.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3gtmbzulv.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3yvrowjub.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3wzroekph.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ycrffqat.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3illokuxn.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3qbzviorr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3sejjhvjq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gjuxeggh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3hvwyulkc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3xzorlhsg.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3spzqbccf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dgnjyzeq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ymctzbvd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3mxyjnphb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3mqnfgffh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3yjaoaowp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3kjeaxdyw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3cvznvbaz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3wfizqqqc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rrkwahxz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3rqztksez.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ixbitqrn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ffpmbrqo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3muwadipz.html


<!-- 参考信息 -->