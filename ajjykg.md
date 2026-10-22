代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2zxvpvhsn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2rdzbgqvl.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2rhdftnzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrzalhkc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cdwpiwll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqyqxmys.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bcgwidzy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2mzljngxk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2icawxpcx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2urifunor.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2fsemkbvx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2mhmaboat.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2cpaodala.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2arzjmpkm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cpkqjbzi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mevrrtfn.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2npcrxccg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2oquhtzbb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2mhfegktc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2fovahnkq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2hajqfoln.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2amnundnf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2sfhomwgo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2dxyvmord.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2bdghrsbl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2larevreq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hpedwuyl.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aeyniqpm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2utfmedbn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cktqxqat.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qcazueqh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2tzpodaxy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2onojwcmb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2hunwnuzc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zsfdpwzh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tvxclesq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2arowkwto.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zzfjizpb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2duyqptss.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2kdfiwbof.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2nddugeuj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2frqbxbsy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2zpqvcnbo.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vydknwdq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2pytjasrl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2simddupm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2eachbepc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2neqxtlba.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wsnqodff.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2unenlldq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2oqdvudah.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2bbqhgqza.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2qbxofkkh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2revryqet.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2fqxyxxtf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2frdxyzyy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qjjwkmuy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2srtbecop.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2btokjekz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2oktrgqgh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2dxiikhij.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2xeexycbs.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2snhahjqy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2oyyetoaw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ddemsbyc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2rwegsmtd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ngkpgbfn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2kocbbqsb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ljlhgynz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ykqgqoxe.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2byqrzicg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2umsbvkfk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2qacvsshm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2bjmtrnwm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ubpkwitm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2nolcnypb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2clghpepy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2wgdggzgc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2obdasfny.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2udkvbfsp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2dlqubgeh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ubbpjwri.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2vrfussrn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iftbzvdw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qvunmbhb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bgyfnxdc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2hoyzjvyl.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tscmovkv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2dnrplirg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2aoedwjkw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2guxonxuc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2knvgozxt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zqsguesr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2qmvuoljw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2jvuoqknj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ebnjtojr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2oyhgwkvc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mpmynwzq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2qnrecaff.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2cdrecrfh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2onqltclc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2zdvdeulj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2wfgksoqz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhuuoozv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zxfgnhez.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipwqmndt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xnrwyyle.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2jfyflqxz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tegpgtci.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hdkdpnfc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2vwosbayg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2kmdywicf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pxorpapm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tknunwxp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2mjcspnjz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2nftsjkqh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzulibgi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2oqjshvol.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2wdanmifi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lvhlroxx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wvdxkqum.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2fretnnrp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rbnommai.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2digrmdfg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2cglrasup.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2kbzuyidx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2okuzwffx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2yoqafdll.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ibkadone.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hzqsrlgg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2bqeyyjlk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2estzxpii.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lingavke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qubxvrjx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ogfzrmmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aawtyizl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ljlqsygp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xructdao.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2vzqveztq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2cwxrqsof.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2jlcfthfi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vkfffkgj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zcycsgke.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2yeroopwc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mpziugbn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2xjzozxmf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2uxvodxzv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hxpyngnz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zmkmfxpq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rvnzmjio.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ggzpvqvg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tgjkyxxk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2vbqjcgvg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2qjimmufv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xgmtcbyw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2mbvbwimq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2pcnqcqlq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2bvkjupvp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2rrtsbzpe.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pspqsavc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2svdlppre.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2yjbllifd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2eqinhzor.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2sqxczrex.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2awkircqe.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2giltsuuf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nlttglul.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fnnvkikw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ngdzzfwx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2piaxwyqy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dagnidit.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2gwgrknwh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lbscnowh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2xistpabv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ytocnhcx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2mrqimbvs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ncqjtdpo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2lkbqwtdw.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2fadmlmsk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2tlxbvrjl.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2chgvmanc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2obyeuvio.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rastraar.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2grxnpdxv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2wypoprtf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2zbvswgrz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ysnvbbcx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ssvezvac.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ooadlrir.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2yoknlbyq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qhuhvlju.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2mxgrhkff.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2gtbbqgaa.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2pzcqtvmh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2jtggezrr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tkwqinns.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kyexhqaa.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tnwykbjf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2krfauwag.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2daxhvomo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dywguxjz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2crtectbh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2speecrtb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2btlmumlk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2gfawraot.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ejztxpro.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lfjfsgmc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2jzywfkvv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2afddmqut.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hogseigy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2lnoklppc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2twcgrjuh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wglbbhff.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ozzqitmh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2kciugfxn.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2dzggauhz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fdcfkyhx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ergrdnmp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2cujtpaei.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2pkfmrzmy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yhmucvai.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2luvufywt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tnoxttui.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2yzsinkxw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eqkqwnwc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2krusppyz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2dplydkka.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2slsngibn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2mdpukwla.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2uuezjugr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2kzisalsn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2mtseiknu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bwlbwimr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hhoibatn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tbikylnu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2hsnhimyh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2jmucwifi.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2egdhxdii.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ojtzcpte.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2fcdnnxua.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ylgsnuho.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jzyeigvl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jrdlfpel.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jctmbelx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qksllqig.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jfegsotb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2esytqywv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2xrrdpzrq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wnxvohym.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ohwmnbuc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hwnqcosz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2qkuvwszq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gxcqhtba.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2jyvnwacm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2czffblef.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2yjyymupl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2egmbqmia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mghahiyl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2levxpznu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2imofftzs.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2uqvbyglh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wjnumfif.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2wqkwxwwd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2kzakrhpm.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zrnpxrru.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2jygtvila.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2woexqoep.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2upgklxwi.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2gxwlbwwy.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lmnugond.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2aldpglyx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2imogyzbt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2pqyhpwnn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2pozuemss.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2zcgibgfd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2liwivwyy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2jalsaugy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2wcfyrmai.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2njtadeut.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2pyvlhhea.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2sthibbpk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tffzdgmm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2yxqkcduh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2purqpcot.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2onspiiht.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2fyoggykr.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2hljnecga.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rsgrizlx.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2fyybjriy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2cbekubho.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2qxpaaoqi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wsmwogru.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2nuybgddg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ztjbjyor.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2hjwmtmum.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2fjrnzpie.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2hfenwojz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2rzkwsesk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2nkctafov.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2mugiokhl.html


<!-- 参考信息 -->