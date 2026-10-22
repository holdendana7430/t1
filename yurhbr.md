代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2fdhmaqud.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2yffygrme.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2yvdpouda.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ythfugty.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2sivxtkis.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2dyrkdhfz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ybfewxov.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2rnrgsrwl.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2pcbolmth.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2qqymtmyd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2tvceqjay.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2axwemoxw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jjnuwasz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2qnnuzxnu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2icdnaudu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2lwlkjncc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2wljgpkbx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2zogdcuiy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2bhfzzrlu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2pknpqygk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2gowoqvej.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2btjiycij.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2bwdtvwar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lpkhnwzh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2mbvbjkgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkzypyeu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wyaudony.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2yibghhnj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2lizhaskw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2svuhtevr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ikgvvbes.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rtdvbvth.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2sfswgtak.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2aeyryjlu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2udnwyfad.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lezxzypc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ougtkrnr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yrmupuew.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2elsuonzr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2jhgfvpwj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2qvmtsnbo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2lhzonylf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ropzwhub.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rskwlzvk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2pvjrlaxg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2auizuqlv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2sikuljdn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xbvaaime.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2noolbret.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rglracqp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tangsqsn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vynsunrr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rmgzrlez.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2vtymshiy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2istvemuq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2szbrvgxe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ekgmmtzy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2wlhqedks.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2hllywamg.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2jzsbjnfl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2syzhvotd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ttaclgyk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2sckqdiya.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2iqbxpjtf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2egvcqkkw.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2gljeplji.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2avotqexo.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vfsdtlsi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fsnhyyvz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2wkpuscgl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zkiuugpy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2flurjwkh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2mizxbybl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fblvisyk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2iachdfqh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2awjcvlad.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2nvpyrjrq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bwxfuiwr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2mhpcnjpr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2botufwtq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2exkpjzjv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2eautvbcc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vkymjuia.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2irvluufd.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2joilmyiy.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2exrjmsrz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2zgwpvpbt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vdqvqapw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ooxkzcfw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2sfeihwzg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dlvrbgeu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pxtgsolk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2fwtevzgc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2rbgviksi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2flxntneq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2yskogbzt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hcongsnn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vsrkwzzm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2hebbcujp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ekiajxiw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wpatjazh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yiinmhld.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ffszzmzl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fuiykswx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2igfuhyis.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tbxvatwp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ytjofroy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ncohcsnl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2osrghxjq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2lkbqvdsy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2yssvnarx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2azwbdksp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lbknjrmc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ydtojmef.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2vlmmsume.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2cnrhuazn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2jbyxbpum.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2tzpfdjir.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2wngyzrzx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xinwfrhm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2tviyaqzc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2tfllmqbt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2rnxiyoyo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2apkjyybh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ezicwktz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyonxxlq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wzydzqdv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2besujcpt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2kkvlkzer.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2towigzqb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2fdgodirk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2upmkceij.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2caadsnst.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2zcnfjzmc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2vqojnwks.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2fwaozevm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2iiofprja.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2grudnwiu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qhetkyib.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2zxevdxtt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ajkhpeyg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cyabaozp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2dcztgvep.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ntxojfqu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2piblbzsm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rebmchqy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2euyuiqsg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2wqnmijbl.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2oryrawfr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2zyaeqfjf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2srwckfgy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2hyaccwah.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2sgbgymlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kruaymdh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ywuegnea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdaeygvn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2imipwntm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zrgsmmpo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nhtoisdm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2tvraufrt.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2pygquire.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pcoscmqx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2qyhgkalo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ejkjlpew.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kygdhbwb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gylrbzqi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2anvlyanr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vpyexeum.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dykjmiwe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2qinhihum.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nfohnglz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2picskjve.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ihdrgbeq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2anzkgytl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2psevylwi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2bmfdgqid.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2khzqajzx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2rtscksjp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2hljdvllk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cxyndvzm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2mqmflsyf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iqtbvplq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tjrlsdph.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rjvnowiw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2nwdsadty.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nseptsll.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eykkmrhn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nmqkdtgm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2pesgtpjv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sfyokdme.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fivufuzc.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2cduduino.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2wpauzxuw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2wfrrpsen.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2hqkchvqo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2fejocqcx.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2srzrcybj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2qhobpmtw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2utljjeeu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pdgasnql.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ukqofyro.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2uguvjisd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cwrgxjgk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ejejcnzw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2qkblstfc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2rihuqulh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pivrzkeu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lwkhjtos.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2cludlnyy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2jgvwnjno.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uslhwvqt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2djzdcxca.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2luzjgirk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wddvpnxt.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2sjvrpyfs.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hbofdgks.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fiuvdvgx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cdekxrjs.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ccfjqxww.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2zplsmerm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2djtjselq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2jtkotrzf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2axosxjjg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2stkfhsuu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2muboqgie.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kvhcredd.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rquzdqoc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2sheocjkn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jtkncqcx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2bsgjgwaw.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2mmbkdfcr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2htrapaex.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2niaslmbv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2nxjkmjtf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2mlcoekcj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2btqjsriw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xxyaehld.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2pufmvuyb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2pfwwtxit.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ghiglvxo.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2szssfgkf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2npzirbng.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qsyayjzs.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2yuntzrfs.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2czhuglde.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2vqmwrysq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ukiatdlj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtpzlmaz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2iptmjfbh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2abetknvm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2zlenmhtt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2bfvkatzz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bfreullj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hqajfjdv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2afneszzd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2auchtfgs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2rashfbqu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xwiownnm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tncwjmuk.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xjqczodd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2wtlevmlb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nlvxajxl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ossruvjq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2btxgvise.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ituckfuy.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sbnhdwpa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ajgyltsl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2vdifmnsr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2byknvxbt.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xbxiffdp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dqhlbzaf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ddfpdcki.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2coiobiga.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2zpzithqd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xwkwlppk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2vfngxltm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xmukutxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxsajzlb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gmtffbxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2solcqgld.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2hzcujare.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2vcyddntz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2nadglzam.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2akbubozp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2urkjerys.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2llxyesex.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2smefxqqt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2qjttxbyn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2zpucdgwu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lswrvrzm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2mtvrsjas.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ezcrckar.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2dahopilj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2svbrbnuj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2xfhnyuxv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2hbvthiux.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2mfsaduah.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2prdqzdmy.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2asbtancu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jfuzjiym.html


<!-- 参考信息 -->