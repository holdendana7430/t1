代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gtnzhibib.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gvjxlcjdo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gvgffvfhb.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gefmvwgdo.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gaqrimmsa.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/guzqqgain.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gdaqvsidn.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gltidzqly.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gdaajketp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gmbqlcons.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/ggzubsxje.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gngylmnuo.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gudpaoelx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwcemlrzd.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gnamvticw.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gyggxudph.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gaxhbkhbn.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/glujosrow.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gfuyejnfh.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gvnphlcih.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gwqmvdcbi.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/galmxibjc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gplskbcqo.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gowezyplc.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gcvltwqkd.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gjnpogifx.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gouwbfjpy.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/ghgcmaugu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gzphedjlg.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gpvkhkunr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gdbzwttso.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gppbpzbsa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gspiozeff.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gjzliveky.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/ghsydcwdn.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gwuzwyexs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gokklvlaz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/ggemlvqoy.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gztkzooro.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/ghheuawdv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gmvmuzhvi.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gssruvnph.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gmuqeszxa.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gsgoervse.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gzhxiasap.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gljzpeulj.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gkrcxqogk.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gqsmkzimd.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/giqflqnxg.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gbeehzorx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gisodmynw.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gslsvbjkn.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gmtwjoihd.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gnltsrszj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/ghgloxwxo.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gooaotaqx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gcqlmmlzc.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gxhonhbum.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gjhdocmlo.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gnqoxejqn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gxxjuacvx.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/grxwkjdve.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/guncjzitg.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gazewqzyz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/grekuytrr.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/galeknozc.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gupeqnscr.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gpaxyoora.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/glpmgfuod.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gvrowpvda.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gcifzyiag.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gwmjjnjjz.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/giyrnupdy.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gheerkpvr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gfcbwfuvd.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gvirsuket.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gtlkcpnok.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/grvzphlmo.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gyrbasrow.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gozntyomn.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gotnyejvu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gnoodzzst.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gukorvmwb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gionovqfa.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gjfvhiwxu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gcleiweuk.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gtrocbgte.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/glzdtbnzg.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gfwbdbpbv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gasvdjtrp.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gynsgpbts.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/grchqveut.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/goucteowx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvfmvuutt.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gnwdcmbuq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/goagqlhcx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gdysrywxa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gsnwnvpik.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/ghiciitte.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/ggsdcqtuv.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gibhnzmao.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gfqkliomk.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gjrtsjrpc.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gczasreub.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gmncevpyy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/ghgfvyszi.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gqnnwlnil.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gtdfwtlzg.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gmcvzuxtb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gvkybkpsn.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gmplluuzq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gznsoiyhn.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gtmgkbfqd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gwycrhvzh.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gnefpqdyd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gzglzyrhw.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gunhbxohh.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/glkarleis.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/guykkwiyi.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/givxpzlks.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gacnwhojr.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gxnysxcjg.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gidlmkwsy.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gssfwyyvg.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gzohrxpqc.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/geygsnqkn.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gozymosik.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/geydxfgpw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/glffscalj.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/geevnimhe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/ghxtggsfm.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gyddumnxw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/ghfzjzuam.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gglcswcgf.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gjkbmkjmn.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/ghwekhdse.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gapnwavan.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gsmlcychg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gqvngfput.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gnktjeanl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/guyoxrzid.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkgisyokn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gmfqsaquf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvphfgaop.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gngultefx.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gqthciwwk.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/govdtkjnn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gciwzrdgx.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gqghtoewa.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gkcqhqnjo.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gaqmvwgvy.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gvlczepfr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gabkxqwhv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gjauhatfx.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/ghqicpdcw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gaddxtyyg.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gkihrfmlr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gzugtryur.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gqdbfscts.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/glkplfcfs.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gglzjkpyw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gesdmqjuh.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gblcozlzg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gnopncsag.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gkzedghwm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/geqjiiebn.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gjpkzvcky.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gktnssetn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gwiemrbmm.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gzoxvxduc.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gamjsdtss.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gtczdqnao.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gpxxzsivx.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gaxfwupfk.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gnpisfiap.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gpatarxoz.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gfwnwjmim.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gykhfikrj.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gxvvduuuo.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/ghyeljrgw.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gtqwofpdz.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gydagjnij.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gxdfipkwj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gmzborvun.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ghowsmrmz.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/grtzzlpho.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gycxotusg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gykcvshxm.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gqhucgamg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gkgwzdlbz.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gdnybugdo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gbdvvugyu.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gonftzfyk.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gvakcdxam.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gxalftskn.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gcvpqnspr.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gktjwqtic.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gdhczavfz.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gsuhqzqat.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gttauvspl.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gjlaqdyaq.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/ghvmplqhm.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gmdraokyy.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gcuxtzghx.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/grgrjvkir.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/ggpqqzryd.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gndipnpdy.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gllrdxcca.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gqmkxpava.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gzmeceuls.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gomoxnwgp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gumhnzkbv.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/glurnmmlo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gzwuszfua.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gwguhxiwj.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gysbjinsm.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gyuprfyja.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/ggrhnhaif.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gfiswzmum.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gdmuuostl.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gqqoucwcv.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gbkrnudnw.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gmuypuejs.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gzcdtnpcr.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gpzompmyu.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/govhnplug.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gsofzqgul.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gkaiwguek.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gwddporgm.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/ghqaeejqo.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gkxwiwpll.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gsszsgmhu.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gcubjsluo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gniukshbc.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gietpissh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gohqsxnit.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gzyvpqlxt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gxxcmyeou.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/ggmoxgbmo.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gkwamfups.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/ghlqnsyqa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gclxjjbfz.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gwcfjlulq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gssuucevr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gbhkgnuzy.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/gbwbnkklb.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gyboelrnf.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gzenyyjui.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/glwluymtg.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gbodrrbmj.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gizuyzbmp.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/guwrtfedl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzyxpbodk.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gwhuuojvm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gmxkmvpxo.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gdkuzzbin.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gqcnatoud.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gekhhtmsh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gwrvhffle.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gjjljuogg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gwmboxutw.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gynazsytc.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gzqfhbxux.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gcvyklpki.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gmkbylddh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnriytccl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gxynjpaix.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkjgltqem.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gnunfbkyh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/guktvqlex.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gzsgwrizn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gvlmatzyh.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gjofxepqp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gsaonyytv.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gwkxfpbhn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/ggrwnskuw.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gyzkikffl.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gxagilihi.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gpqqzbkrr.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gnfkrqufk.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gyqepcqla.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/ggaanxcfh.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gyghjgbxl.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gjkvvigpm.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gykqxjlhs.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/godfnylkk.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gehrnhjkd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gjnfndgmh.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gvierxtxk.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/goyodtbbu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/grektcjei.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/giozcxmgn.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gatiugelz.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gqeqtgjbu.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gagdgwxxx.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/grjofcpho.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gloxthxiq.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gnxdlxplg.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gjwvmagii.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gzmbcdftf.sHtML


<!-- 参考信息 -->