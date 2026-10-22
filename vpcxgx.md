代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2henwdxhs.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2itlukecc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2voobrmzo.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2woxuhbas.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2obdxmvir.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2bjjzvtro.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qqqjsroe.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2paprtwrh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2aqghmooc.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2vjiigatb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2tlafdaxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtojvduw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ngrpjsoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oewmiwed.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pvekxqwi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2sfbmoihz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpbejrbg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xkugzcoi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2jvmamfqi.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2hdunyksq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2yqtpozka.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2odvljpyb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pavuytut.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cwudyrac.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2cplbzser.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ylaotkkb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2yqihfncf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2nfeopgec.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ftratnrv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2uhkcgmww.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2gtquzkyf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2fvhexnbk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2txrlpckm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ehcauuvs.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ckopatuc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hucsmmpg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2jlxozsci.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ajskxwcl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ryscjbsi.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ndiwgcwu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xsyqqudv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2asylwtqt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zcnwmxoi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2xjpurnhw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2wvwqmtgw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tvcctziu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ypizbvci.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2rhiiipgf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2crewbrpb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pyhbronz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ckmqtonb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bhgdzgem.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2vqmfxnsc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2qnyjeqvp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2abywamak.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2slbucbvx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yvhmwhgg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2nrbmwqrr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2omjlqodl.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ytfbyfmr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2uiumbbjx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2kcqaqoxd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ihobbzft.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2tvgvsnph.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jzpwqtnw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2snpgcqbg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2tekwnbaj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2pwihutxx.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2mptmwupc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2pvnerusz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jzkonkhu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ziivukfg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2bqqlgvht.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2hybmznnr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2qwacfkgf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2oodeskzv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cvsnvmur.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fdqroezx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ypzyrhrq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tpiwvdor.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2qvggboft.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wkgmhbfv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dcpewegt.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2goybpmnd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2evymcubu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ixgwtdqg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2imwoytwo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jgaonkfn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mibkkjkr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wslimeev.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2hfsedmnu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zbngldkk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2tgrqfykn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fpinmjsn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2goignltz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2immnlhhx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ceitoatg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2lijamkho.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2remdetwx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uenunnuo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2buxuobfd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2swbnmuyk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2elbnngoj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2qhbzmpcy.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tmctrezg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vzpruobr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2vhioknnt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2laxfebwz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2navpopia.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2drciujkd.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2uhdwauhd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2fegfxckz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2wicmprno.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpngyowp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2knfdojiz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2sifkgkbn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yirrohki.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2emvnzxif.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2moqxxnpz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2oxpxkete.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wqqyvctr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2phnmkjgi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2mlxbewva.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2mimrotzd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdurgmvu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2xosrrzwr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2fmproicc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2kykcwvtl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2umydpkgz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jyxvrtzx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2mbrmamda.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2xcdrsgtf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2aimimear.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2urvbsldl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2nwlujtbr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zjnacuxp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2cbbkhvcg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hzvpfkeo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2shmballj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vdqbfvla.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vgpseary.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpqoxolb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2toutjidt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjbsmzrh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2boicsnzp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ewkktxyk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ipkwjkte.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2mccoyhob.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2mjhcxbyv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qyfphcec.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2yntkporl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wzoaizgj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xohgexmz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2bssoyqeo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rzjmsvhs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ckdmeuxg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zcnoshas.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2vxlucfnf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2nxhmvwla.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yihwpbhy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2pqlgjkyi.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2evknaffd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2jbvxnkip.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jjihwxnf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ipjrguhr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jmyawate.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2vhzsxdbk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jrvawdqm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jkwzupig.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2axhoalum.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2xaebiqvu.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xpfuojhz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ofgcpevx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wnvjhpnc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iiylrmhx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iwesaikm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ujinkxvd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2jqvhbcjk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pbjvolqr.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2qtfpgkqh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xlimzbnj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2mjlqzwcp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2hqwytlhz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vlsiovfm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2cjmyiyzl.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2gyalbbuc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2eiwqvhor.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mtpxxglu.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bbadimpx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2dizgrwmp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ccmiysnr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jvsabifz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ynllrzks.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2sqplksat.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2czwbbzlb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wnzrohwi.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2stpqzgzo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2luvjgefa.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2uvaauwmc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2xcvfrnkz.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2uistmbbe.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2bepmzwxv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2uvqvipbg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jttktxfn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hxrpqggp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fioxddhv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2jhelxkjw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jggisenw.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wdbaaouy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2nvyczrvq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2thsvonwf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2mqbwvhua.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2kscxcnlw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2sqnlqdwu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qhtqxxfj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ejenxyax.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jzovwvgw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2pmpnorpr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gjnkfvli.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2qiexscws.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gsrrzufx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2khjytmyi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2wpxweiwf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2dnymydlq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cosszsgh.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2lwjpxxdw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2rohdgqxl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2cxhiqkki.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ofkqxmzh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2jwqorcpe.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ykyrxtro.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2eiygdjxz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wgrmwesn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2zgtwdjhn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2tzaokync.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sewjjdak.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2mtujsmiy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2xquyxruj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2qwcivwvf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2mdovrzgn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2tpvmyqdx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2akgybrqo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pktxvkgh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2bxplitea.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjzmwoaf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lkbjyyhs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rpwhkedz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2abbskcaj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2nszhpgqw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cporujug.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lcdpimvv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2riejmvqw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2foyezdgq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vapjjbgz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2tihautbd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2srsuhmco.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pkadacbt.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ctdfkmpr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2aadhonih.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2tvkgovqa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2obfejrtc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2pkvnxtzx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2myvxoxxm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ytpmvmzo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2pgdfiusd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdozhbnl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2auikrvgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oogvyvbp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2yxrwnrga.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rqwiqylj.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2itfhcrqb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2oyxhagco.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ghvfoybj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2zuaglndc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2wrvqjmvg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2efkuouoz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2oxdrxpyi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2httlqgdy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2xpugntgx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2clkyrksd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rjzctugu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2mwbllyri.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2netggjqo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2wciferuz.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2dbhgseqi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ylsacmlb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2qysogqkk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2qxwrkvaz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2apwqjfod.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2yeuncvxw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2deftlmnp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2iihyhkee.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kenpxrnw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2dbfxjcbe.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2gcjsdzlj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qftygffe.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2gjhevian.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2fqruspxn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2fqbxebee.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2fxmoqxbd.html


<!-- 参考信息 -->