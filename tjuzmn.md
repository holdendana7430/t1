代发 wailian999

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2afxylizp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2nklkiakk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2dvlywjbf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2nwdurgas.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2tasmdqbt.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2gavztmkb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2qtthlyov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdtmcbif.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2esezhraw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsvqucdn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dnjgbnfu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2cmplbufv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2vntughwa.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2fjfunokx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2pnxbeepm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ozkygxbd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2rleijyww.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2kotjfqyv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2nraevkvd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yficjzfl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2romheldd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ffrilugq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2qvcmzytm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2xpqnxwir.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2jrlezseq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ecchcsvh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2lklnlqqf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ghyqzikk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2bqvpankp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2movyoyzw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2tmsiqqnz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qywiiqwe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2nfcjbkfh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2bsasvoso.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fojkwrpz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2khfmjqrs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lyckdmzj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2gokoqpkz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2tenbytnk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zjyvujnr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2tzsdjbrr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gyqyqqiw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2vddoamxm.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2figktjjk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wamssyeh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vbekwhdf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2jsyahcah.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2atgvhxqq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2daofkzhh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2qotiucrr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cemxtttc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vxwtzvsz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zvzfeeoa.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2jttqwhql.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2bjuzecwt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2yoguzxbt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2bpitakrt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hjdvmgds.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qxhuofhj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2qpmuguwx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2dcqyvpbh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2xojzvzmq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2zbdfbtaj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2rdjwwmgi.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ymntproo.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2rtzdlanl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2alqplnre.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2saropute.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2cwlkpvxc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2mizqiycv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2gmzfsczu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2htjbtrkq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2srlgwncs.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ssnnmpjk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2mgwsljbd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mqoqwtiq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2trytpnsx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2afrahqhj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2upiazbri.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2vhxkbncu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2zkcoxjaz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tcsyoqrb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2yhvagosy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2vjcgagux.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2zhxacalf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lvgrbefj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2yqaqpuaf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xyyuamod.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2elxsgaaf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2xxayeukh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tlmxzoyd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zldmsvle.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2bwisqtuz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2opemrmav.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2hkcpxgau.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2otveyaej.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2gmziuzsu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2mkkmieai.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2decaeadt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2vroiqlrs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2stxnjgrl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ftdryvgr.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xrbwtbhj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtvqdlae.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2woztgjgv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2zzcmxmid.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2pxumxeoo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ugkrruqt.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2izehrdkf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxlakxss.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qaahrnmi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2brlfbxwi.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2coprctpo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ypziknom.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2bgfmmalq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2edkdlklw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2knvgiejn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ydpglvov.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2qdywtaui.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2waikgpeg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzkecoxk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2deowmtgz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2rkgawicz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2zgeqxxdu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2drugcpsz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nvqpypjm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bjavlvef.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2noxxzauk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2tlkcxgpc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2tzmsftev.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ongdnnhz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nvdgdhyv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2beecgepb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2xdduqhud.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2pnflbjcv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2dtntimvy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nggyzqdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kqbgcgyx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kemlpqbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gxyvhugi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rtdtltkr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zzaknyrt.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xfekhxza.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2wknvstew.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xqslusuj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ndqsibxd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2tqizepfj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2yuxcggpg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2naullegj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2qwoglars.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2shwtnzje.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nrrumumt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xvhmavcs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mpvkyjsm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2qzzckmoi.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ejfaqhjf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2xwcceyju.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2uwtfjuoa.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2nurhbdnb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2rvgebyif.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2gkntupkf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2mvyqszef.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ubtcjkmv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vdeusiyo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rqxrilik.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wxbjettl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2zvtietft.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dsjfyrrf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2fyzuklyp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2egzhtjjj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zzilakil.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uweucszc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2jtfozshw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ryikbjuv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tzcdglyl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2vlmoneio.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2plfkhmug.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2hnwjtaoz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2drjtppfy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2olmsqbit.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2moybmuyx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2drcsammx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2rmuesssy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ufqtskfb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fgrmeibs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rvhbslrw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ttkespyz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hnpmmrbw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ixlipuxw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ymehyrtj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2lnpzkdvz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ahrwcvip.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qyphzrzi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2gmbvvhjk.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2hhebmrdt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2drxftlli.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rzrmeoqh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2lxhbjoyl.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2mtfgmmtp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2qviuftcb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pjjswkro.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yesxmyqm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2gqfbvewm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ypxicgxp.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2jwolegdp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ccyrnqiy.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2cnwrwami.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ugdihcpd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2inyjukzi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2altttwbn.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2drlyvqwl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2glqloeaj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2gcojptbm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2gyfbatin.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2xrknsreb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2mxyspwrl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2atzucjaa.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2hadiwbny.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2bifdbwjf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2olzgoefn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vcsrowff.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xviipzat.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2exutifai.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wcnzmknd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zdwoerht.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2zleoyzxu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2miaffrao.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2nwuxdwbu.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2codfepnq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtcfmzcv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2pomdyots.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrkutqul.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2etzdgorz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwiawjbz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2csdxxdvt.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2dwrhiibk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2lfrusnac.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjlzhhxa.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2psbqxdfz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2iizskbil.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2baehubwc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2amravhfk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lvsfxydk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2pzowlpvw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vxgawicw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tbbycmld.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fqqdmqov.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2pyozkkwt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2zyumppnx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jwysmgel.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2tgmudsyd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2tqhafcuv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2pxlemntn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fsettoiv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pwczyrut.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2jmbpjhsi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fenxdsmk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2cfunjeio.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cothhjfk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2bgokxdpi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2zlpqswwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crorgulo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ghcgehyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qaasldgp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xsfqsfvs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2sgnqvdhl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2whcwdbqo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rdtocwdb.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ikilyimy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2jzrzcyms.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2lcrukivo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2lqpmoriv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2avlfprgd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jghxyhcd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2bgkaenqh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2wfyyigtf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2qtuoqgss.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2eyqrifio.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2cxhqyvwr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2udecrkak.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2lckshrux.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2uotwfbyo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2qrlorztb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2yfdvntgc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2vjxpafgz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fjyifmkf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2gvnntgnv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2yjqgmbuv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2bbgbzpau.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2sbofvcbr.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2yujfyeev.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xdqtkqre.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2dzkgpsuk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ciomhjue.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2trjfinbh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2slufhbmd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2gbnssety.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2jcvihsrv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2yghszlzj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ggqcahfa.html


<!-- 参考信息 -->