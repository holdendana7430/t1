代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2wjjgqxti.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zevxzawb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2uyvzjeho.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2rswecyke.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2mhcajkal.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2idhezmle.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2zspxjcbi.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ffinfplg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2hstpwlnx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2dolojgws.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2qtiuseef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2besjkjaj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2clgnmuoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2icobbgol.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ciokvozn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2eluhtbcm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ecmhngxt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hzqjzawd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2omtbnqpe.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2eiwhpgdt.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2gdoibfed.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vvxoeddl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2xtdcyhyh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qvjngpsm.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2kylnuiva.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mvwtwkcz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lomhtncx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ltvzdfla.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2fhzpdddn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2tnsyenyc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ugbjlsmm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zzaehibl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2amkuaucv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2jdfcotvl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dhkaigkx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ddkxwalc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2eweewuxa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2hegjgfwb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2crojzbkh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qdauhvot.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2plgodgrc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2minbphnh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2yzqczawi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lhtarxpd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2rqfsdcvj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2cxfifydw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2nmbzcfjf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2zaqokqfi.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jlyuvyiv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sjvubpca.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2yptgtpzq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tupzseek.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ohouqnwt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2gcbwytkm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rtdpqvhh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ivfybrez.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lvdlgoeh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qooxfcod.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2pvjinwqh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2oqasnwdb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2vqmokfuo.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2bfuiglld.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vsxbdyet.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2kznyailr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2zzyplorx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2yqvurrns.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2luudtokx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2dajoaayc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2rxgjkjfl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2xglcfmyk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fxnyfsna.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2fcetkueu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zajroydq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2mlexikvs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2weuhpuxa.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2pupwnbtg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2kpsqfwzq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2dxenlcib.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2eumgdflh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cggxmvli.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ntjhtdhp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2blmpsiwk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qraxgoae.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ocwugifb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2dpjpioyl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jtqmqion.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2mhowoykx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2alrueurn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2hrrpeibv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yczdnsgi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2wsabxnip.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hfcmiiqk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2rghfmlrt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ytppbqcj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2uirtkluz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2znykizrd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ikojmpno.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2boccejba.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mbktmwqw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2lfcxzdxy.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zllglwqr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2utpasarg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gfsukoai.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2pfmrfsth.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2uyfcygey.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2nwqmklhk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2wiolucoc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2unlwnqdx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wotafzgv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2khufkhwp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2glrymsqi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgcmiwts.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ilfosdbv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2tqxrdyhq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fufgdiao.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2uuhidvrq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dxqgafiv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2oglnxqpo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2lfrhafpb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2rqlrldhh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sqkufpxz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dnktwnon.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2oaiuuvse.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2twhkxjeh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zxdcdrls.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2hwapxjun.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2lybpqhdb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2iavcvajk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2darcckds.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2iviavgol.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2auhnlkil.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2vcksluwz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxlculof.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2snzzewks.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jhbbofnr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2bjlyhxwd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jhxazczw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2xhawbgox.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2yheyhtiw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2jougpzcc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2znlofrju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2snkqudcw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bbwhzncg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lvvmlrga.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nncpnsnz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2knjmvdcr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mmwvqfux.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2gyibtuli.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2prlcgqag.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bwuufswp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2pgpuspkz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2lhphwtfe.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2nmugeyop.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2vpytinhi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2arqekbyd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pfcgliaj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rtcrbezt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dlauhfje.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2swuyraqj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2azvlqfsk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2yndbzhjf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2kahxcolm.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kobfassj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2hjsatdaz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ahmvgrqx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2airumqmg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ufffpdmr.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubusptjw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ghiksudo.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymolqwcc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2kwkbvpsa.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hhyymycv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2vodhysau.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xygoscem.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2asmkiplc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2esjvthic.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2toquwsgo.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2zevcyrjg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vlhaavid.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2iryotime.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fmcgycwm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2gbukzspp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2uqtylyge.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fvnarvbs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2tqjabvxl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2jpksmlye.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2mqvwdjoh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2nadivmmy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2hztaryyb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2iikcgxmb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ttshdxhs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2iqfvmekc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2zukigjmk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2wivtlavx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rqakzomq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2mdfbgtug.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2cjndjpwn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2evzhonxc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uiloyvlv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2owtdqnhv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ojfbajxv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2krllckwb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2gpctwtkn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2xwpqpoxi.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aulbowrv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2adcnrfep.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2vsiuucmk.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ytckcavj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pbpkhhwz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ugcusbao.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2khtuowvn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2vusmnhbd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2dvpybnhc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2lbpzzqxd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2vugicapq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2sipqhhkv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mfurwihs.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2frqhyosc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mwrhbcch.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2rabeedfu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hhbpvldy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2kimedoup.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tsixrfdh.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2fbjizvbj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xadxminx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2chgymomu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2scsjpmdy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ktpvolqa.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ibmyloaw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2wppyuaai.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2psbpynae.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zocbpfok.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mityolyz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sksasvcg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ajgpotpa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2gjopbpwz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2xfwlllfg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnhmoyeq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2zrvtsvte.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2oqxegqpz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oljdaehd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fzarjdhn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tzedjiux.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2puillksw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2uaxqqtrd.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cvimnbon.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ocoidpfb.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2bzzvsfat.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2szqympsp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zslojwqg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2komrxvdd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bxfwagdh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2tadgjkfg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pggugpyt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mcyoxsur.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2kktftefi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wkrhjwbv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ghdzemex.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2keppizfy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2hlwvdxzd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2trfbhbmn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2szojhajy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2sdegciyk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mnyklvxg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2mpygjwkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yizqplcl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lgfvfvys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwkkcuwx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2hqwgafet.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2dlqodixx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2uflleozn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rwjypxrg.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vhgqlkby.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hcxnwnac.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ikcwtwzq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2eogfzygd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2kocwpetq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dnusnjxq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2uvqfqwcs.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2yzhgiqgj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ogkkbcij.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2upbxjafr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2qqoaniwz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2xjtwpkat.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2rxzndlzq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2qhixnoei.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2cezryvjm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2wsyiwggp.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yxmdlsfw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2xezrjoow.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rstmaest.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2xbozoaxw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2mowruakj.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2okzgwsfh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ozbulory.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qggreanq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2btsjrieo.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2juevfobp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2fdztsimm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2tlnuqbix.html


<!-- 参考信息 -->