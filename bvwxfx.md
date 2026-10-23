代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3obarmcog.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3xonlzmob.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3zmnijdrj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mzevjtgv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3zuyclnlu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3zvqiahdm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3shrkvttd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3zzghqudu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3mxshtley.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3pgiyesbi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3puaoqbhw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3itftngvi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3nypngdht.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3lvhsujol.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3padwetbe.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3cbfztoaq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fauepbox.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3gasbnfoa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ckhzlciz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3fludzsda.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3keizatii.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vcvtkchg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ymembzat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnzpxedr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3mollhggb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nfbovfpj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xjepvwco.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3pxsitivz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzovlqnf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3otpstmmf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3aroboxou.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mdbtfqvm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3lnovherr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3rmahgtgg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3urjrfwdw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3oatbbucc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ngycwlub.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3erppuuml.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ghvctanl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3zspsxlts.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ywnbvgxj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3gfiawtja.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ljoircah.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3cvvudrfl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3uybpyksg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3otbhauvk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3bdadikqs.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nbbvpmvm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3babsmeqw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mrmbqrnw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3elnsocsx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3bzxszgal.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3agjeujct.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3fgetnrzk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3iwwysvrv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3xpchrxed.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3wczwkpww.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jgzsuseu.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zxkcmnql.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xkiiauim.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3dpglgdco.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fxqlkoxu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3wfjwgggs.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xuuapeix.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3fgktjwot.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3oiufnjos.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3udaezije.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3xjcifzit.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3umeuorqt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3aotnbuyn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3onlcmdjy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rhbrhfnc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3kqykejue.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bijepunr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3pnstqmzn.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3tbrehuxg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3uqdvexot.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lcxynquw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3llzujotf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3fmiwwlpb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3sewojhfq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3nurzekjs.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qbrljeia.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3inqugkes.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3cvaiymqd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3kqrmjcwf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3owlgsoni.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3dcavbdyf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3enjdyryv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ragbbzdf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3bsmiifxz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vcgqabff.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3rwvhagwe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rezntwtw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3hzrorckr.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3dgeenzpx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3jontsled.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3paeqozhc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3jbxgrqci.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpgxkvhx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3fogstkvq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kzildvam.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3vzafdzbk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kormmjyp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3atlhfcal.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3acatazpz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3xhfunmbg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rnlagzzj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3wwqogdqj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3lkgxzcwf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3dqqimbxk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3znywclyu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kphstkez.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ohhnfqlq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3rqucyivb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3oiicmrvj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3uitoygfi.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3asyboedm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3vmzbkomw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkwpwejp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3lsybyban.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3zmamcuge.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3hfvysrkq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qefqlopd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3txbsutyh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3nifngvhl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oxhtswwo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3gmwgxpsy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rmolmpyn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3xsbpamde.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ehhszcpx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3khlvenvv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jddicysx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ndpwlcaw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3omtvbcgv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ojrmvsvr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3wifwhbpz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ezrgmiai.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3wvnowqgu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3apzfgzri.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3snrutwii.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3nszruutt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3vvaqnvhm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3uqhqxzey.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3jehdlotf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3blqgfypy.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vqkziffk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ergeabtk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3kkseqqiw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3negajqpp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3nqildwik.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3kuzaqmft.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ysqnildu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhjkykmr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vmesxkem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgducmnx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ahimuicn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dvdzmyob.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tjyowmar.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3zzsispdd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3cjuxbshz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fulikrwp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ianlsilw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3dxbhorwh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3bbpikkpn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3slhirbhn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wsvzbdnm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ofyawxwr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wwuesfya.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3frvfhgmf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3clzuutsc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3pcivflll.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3jyynwsxi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3wljrwgmw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3pomudbap.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3jifkqspw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3fqpilieq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3dajkelco.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3wlxfwpjk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zjemxwkt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dapthcbg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptenoxew.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3gtxnidvg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lrjaiygu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3nlngoysc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3rvxjlrrd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wqqmadpw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eqkqeibw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3unzcxsuq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3zluvirad.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xxqvxqvm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3hfxbtviw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lbfyavei.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3hhsppbdz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3iizbieim.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3adolurws.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3laqdazxg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3wsvavyzj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ixhyrryc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3skovdzzd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nwtwblik.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3wtkjbnvf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bfcaroyn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pqrycaai.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3iwgyunyv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3itiqqwmb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3sjlkiemg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hhefcsxo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3qshzjaay.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3pbmfkvtz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kellljgu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xikudkfb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3nirxjybw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ragikghr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3kocysqao.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pnigxtnw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ruvywern.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zpqsvfeb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ipajojfw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ltzejicc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3qmopoces.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3crapmfyn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3vlumhdyt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3bmsjerwq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3gsvzuvim.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3mtakhfhq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ewsacssd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3jsxujwda.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3sxbzfhwj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3zkbpgysi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gtpamuvb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3brvrsrhw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tgmrddzd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ldkrjrup.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3kjkppace.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3voqvppdn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3omrugqwg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3yasarczb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3kutzqebh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dajqgrlu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hfjozgdv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3clhmhubc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3urrlcpqb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulujcogd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ywgulnhe.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3lzzjuglg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3cvmumbve.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3impmudcm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3yjegkbfy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytbmucqb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3honqwztq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3kigwucek.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sbpkqucs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooerpciy.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3urxjaagj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3esimjyly.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwtsruht.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zrtvylvu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vrlriyyy.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xysougry.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3nqkitcpp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fldeejev.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wcmgjprq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gtogvxcw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qnhprjyd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3krajqdxh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3nlvxphdd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3pxujrgpn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vqlywbno.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vlguayir.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jhycqton.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3kjtjxgnu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3dmbhpetx.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3eclluhcl.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pqujbipf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3bapgnofj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3dueosvdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtrdftas.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mracexjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlrdvfyk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3lksnjzla.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ykzzmbpd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3tppzzoft.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3znxujyzl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lpagzgik.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3uenjopme.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3vztnekha.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3mlintxtk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3rqikohno.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kvmhibbp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3exspcgsq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3kxrklzah.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3mgmmxhry.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ncnqjrta.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3eflmekrp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3sikaycpc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3yqdcoked.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3bnbdaxpg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3jsjljexj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3mydimfca.html


<!-- 参考信息 -->