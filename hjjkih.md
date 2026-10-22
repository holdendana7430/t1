代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2raeskvso.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ionkqnhi.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2tpxckiod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abfxboqk.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2drncnsgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwkrzcgs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2asldtgym.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2qajtstfu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2hcotpliv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hkdjgnmo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2bytqnobh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2nbaxgxwx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2owurggdx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2iolfbmsh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2noeoncuo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2snjjspvc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2oqvopjvw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vjrtyhhz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2rfaxqkcs.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2uxaovozi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2kvosmrxi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2surdspzt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2aazwtrad.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ifaswlqm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ntxlqqdg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2yypaptuj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xwlamtvn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qlxckidt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ealqlghj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2yxrdnhbu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zkbbcdna.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2wttgdhpe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qaxrcigm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2znvrcfzw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zviekhkc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wozbsaad.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2jllrgbpb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zhefflmo.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2lkebeqtn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2hffyxjio.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2mwmipnmv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bhihyjjm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2vdloomku.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2tcxlpouh.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2vrbtyezk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2tygrqnyd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gcvcxpaw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2eounynfy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cihxaybz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2zigirmcq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wzabafsc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2oiavwitx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2mgfjrjnc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2tafxnacr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mymkoepk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2azzoywfi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2odlqvhmb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2pvlbicbu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2dskqfezz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zkaigwfl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2gmbmxalc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2cgrfkhja.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wkykynoz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2hwjowwbg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2uciqykbe.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2vzfcvhre.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2edlueuzf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ycrleutk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2luqrxrhd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2iefhjing.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2rjajwgpi.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oviosful.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2bnnmvoof.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgmptdug.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2kilbsdeu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2vzyzvjbu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2cvzjflkd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2oeazyqfg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gkfxtayz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2btmpwaao.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2kbrtwpwu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aouycqxu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2bonyutim.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2phzoumdw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2oxqnnmyo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mgzoyefg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2tdlibgpg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hpqwslop.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ydjriqpi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ccjelrop.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ellkjbmu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2dyixdpyd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2znkkhixj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2sefmcite.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2xvckggcm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rwmcngpd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ibkdxhyh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gfyxwcyh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2jxaelzgb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2pyhxcubl.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2avlqtvyn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2jwvtgazj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2xlqqxxlz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2dnfuitmz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2elzpssee.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2demlzhvp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qlvndnwq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2zcgnmjvh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cqtkyrft.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wutcmorm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2lzzwxwgf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2xrhdlpak.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pqfkpqyp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2bczhfbbl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2oknxdcke.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ggebjdbb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeqeanil.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2pqsssifu.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ddwylihu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2qjdeuuno.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2mbmvgzsn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2pnfdahkj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mtisgblw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2mpheevbi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2puxrxbhp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2zigfeauk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nuksrtqu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2spwncafj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2klygzioq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2xlevrkcd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2jeqecvwo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vfhjhgeg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gulzxrpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdxhdkqt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2shvmmizu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzgqjlat.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ppxmvzah.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xhjbsjde.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2hvrntiex.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2iscqojvq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2hvtucwks.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xyhvqsdl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2hfnhrnng.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2nozyzwbf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2adrmahtf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2drlwphtc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ucxdagdu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zrwwdhcb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zdqrubhl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ucjnbprb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gjrchskh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fcxrwlrx.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2pnxvsdco.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2gucavcek.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xpefarcw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2safmygll.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2umrnysht.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2lrooarjb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2pqynlevg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xghroxvl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qzzwwmxw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2expotsaq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2eejsyitm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2snnwqelq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2teeufazs.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2doyhrjuz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fovekhvn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2akjfnqdy.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2olotjdtu.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2jrcgerfd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2aiwlrwdj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2vkaahgph.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2onwpndgf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2bdzkrtij.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2hsstqqcj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2frygupau.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2srrubfsy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2siaxjudt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2rgvewosv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ssnlqrsr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2fqircrzz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2xvwsjdmo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2icshbvfc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kdpikfpr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2evupvris.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2annuihue.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ofakwhzu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ijiotbol.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vfehqcop.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2jhxvqfkq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2slihirix.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2mlxgukhq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2wnofptqd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ogufoudy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2pvvcwmxq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2fwakjqic.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dmvxautl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bvetutbp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2gqgndgmz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2eaevhrfp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dszaeojn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2vjchktjc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2axxewipw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2gfopklgj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zakgcbsy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2qdobzglk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2hghnvmtl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2hqilfryh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dlhaxsur.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2tplgmnex.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hrrmcpyj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2gsjhwnhs.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qgdwatqw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lfungwhj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2jmooyoip.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2lcivnmhz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2euimdupf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2zmsusbjk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kxhviabu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ywxrwcqh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kkxidgcq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2dzgbqmqd.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rizrccrs.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdarsdtb.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2nromuyhf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2igpojasm.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2hheslsuz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2swymiaqh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ayfuyfzq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2aygbcird.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2bxixkkek.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2uvcdpobb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mpjcctrg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbndqidm.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wcptmjem.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2cavrhzld.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2xkccelmk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fhntplnm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fqijumys.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ixxadpyq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jzkondnd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ozuaojpn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gglgnarr.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2nbvwytqs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qhrzvfls.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2cpphdouy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2hwgorkuo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2qqxcztfr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dnzdeocz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kftdoxkx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gslwanxv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2npdtvvvj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2wfpvhegs.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hqiospbp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2iftfaeze.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2yiltdemz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2svwbpwka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2urmpefaw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fktgxidv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgncbbro.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xovkaivk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2liyqxiqv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2qfkapfrg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2uwxamthd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ovmunxgv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2rrznxohq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2opminikm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2wmzoqhon.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2rphyxcpi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2diabicnl.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2xvkqqixc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2qufikdwd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2xoamrkia.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2pfyusiyk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2wcakpoeb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ijqkfpdu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2zcdjmmkt.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2vttbepxl.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2xzcnbgcr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2rbaaynmp.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vorspjtz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2dofltieo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2rcuoureh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2aixgnpag.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2xpdenfgg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2pjllponv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ipibdgdj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ccqfelur.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ofocyewa.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2qhdpgnld.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ayueazos.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2uipuzgws.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2sutpavbm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2jpaoerpq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ltceijmh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2yltxunow.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2svqgzxvp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ydfyhriy.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2mzzmvtfa.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lapszzff.html


<!-- 参考信息 -->