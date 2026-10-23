代发 wailian999

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3psntzcpb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ksoodrvl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3jrojdqrg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3lrtpidln.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3djiwawiv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3whaxrnvl.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3lenbegah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axdefppc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ihjzjqqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhlgingw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rmrrjnam.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3zlnqnkdu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjfsciit.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qpshxedh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3dbsnajyo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mwyyzqcm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3yvukwvlk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3qmizbxwp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zxzctlxp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kvelcaeg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jncdbjfp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wbpwaiwk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ubdszvht.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3tmfqfrgd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3hmitavji.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3zrxjnhlk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3khtoboeg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3hhsiormr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3hijryuns.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3xmedbabx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3sykgfnqh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zfmrdizs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ndfrspqm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3lkigvevh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vepgzhin.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3dajgkhqb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xuwxtbbt.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ylbjxzfs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qgnxqecx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3tjdmzfoh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3vfsdjmit.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3iazctamc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3yievwtby.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rogydhun.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3apxhyagv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3twtctfqp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rhmuvgcm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3drkinzdm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3qekkmews.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3bxmrbhon.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cupshkrl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3dystfvqp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tdaulssc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3wlptcixe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ybdqtsqg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ouxnotal.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3oripdggg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qnzvmjwc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3npywtdfo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3lupwqezj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3qalylaet.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3unavdfwr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3gucsmrrk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3jjgxviox.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3furqexwn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3bvmlbibe.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3myhtqphw.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3yabvjvnr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3qklqkgzo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3fbocqpgq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3pudhpddi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3zyhunblk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3gnnbkgbe.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3zvdfeuwm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3mqmopbnq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ahrbxixa.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3qwhyjfuh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3qzckwtfr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jwhyrczg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3qinpzudp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3smyogpvq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3tusiegif.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3earqsfut.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xksjmtxp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3bnbilowf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vbikfgot.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3vyuugcpf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zyhuhmag.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3gsrqvnkm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3bxeunfwz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3hrvzakox.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nlopswrf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3uqyotzmz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qwsothgv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3rxqkusnu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3qhrlvome.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3cmxxkmsy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3umhkmwry.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3wfsyhzwq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3axhjllpc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3kduszfai.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nfikxgau.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3lsrzwltm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3iyopybqe.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3airgibyy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3rvpsefkz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xsmrwwri.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3knglmwew.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oyklxoke.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgqphkrn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wotyrrka.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3pextykkn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yczqsqhg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zitejoep.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3rqlkpbdr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3bvwqsmbc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gassewpg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lvwdkwaf.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3mugmslkr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3kknqcupo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3cbcgdeva.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3afqbfdzp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3lzubwkxe.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3rupydnos.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ufwxmlyp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gqgjnofw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tssbjmuf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3dbchgqfe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivjohjbt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3cmndglnt.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vgcfrlht.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vkwbcmiz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3imsejfqq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3avttyybw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3wukveiuk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3tquapiws.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wqiyjgeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fnqjhosg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ndxsbpon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsgzrgbu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pcqnpayy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3itxuhuiq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vexnitbg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3wgtaidnr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3dwnsbhcd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lukgzhmz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3esaqmevv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3nqcjuilj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3nkroucrn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3gzsmugkf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rsnqbcxg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cuuwepkh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xuqmyvib.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3btturifp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3dbgmhqoc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rogujcof.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3nibikwys.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3popoymwr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cyvtprgt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ofygrqfb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3imfnwcvk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ytsbzsyd.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3uuuobvlg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3slgacchp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3mrzmfzko.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3irpohfqh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ymoxrjre.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3amcgowdq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3amudkecv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ffreczuv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lculzyey.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dflrgtpl.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3rnvspseb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pwbufaac.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xmzshqeb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3eozkahxm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3knjiulzj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3sfmvwixg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3zrpevhcp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3vcichhmy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ohkhzaaf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3snyxrpex.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3uqernqnu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vtnbdmgz.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uydeqajg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3bbeptkgx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ythxsfai.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rkchhwkh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3upmzictr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zgecruar.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3wjukxerl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ejoojvgq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dksompow.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3pmajbiho.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qmrkaoda.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3vnhsikbg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rrgoxfbj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3dagbdjyj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3fncnkdmg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pnybzuej.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hvqnegig.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xqskdbii.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3gmnyarud.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pbhtbeyt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3shytvidq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3gsjxdvte.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3aygtovtg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3sqzhymil.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3hwoxvzwo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3osezlgqa.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ytuyztcs.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3losykcdz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hkmyryie.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3nolelqdb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ymerkfbr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3xubioimq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3klalbsff.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qorazhwm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3nvwkggtb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3pocnbpca.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gkvjhllz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3hveaeewh.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3fqbixuiq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3mfilettf.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bqlepopy.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3iyahuykl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pnfxylsi.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejvzkzxc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iydtlnwd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjbhxybs.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3kkokgpxs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdtggwox.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3byyhpxvf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhebxedd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3cwbvnmdb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3psbmkpkh.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3koejmjcr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wuemvcde.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qznvalzc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3fosjfbex.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3csudwary.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iyztrnrg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nxuzogsb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ibhwfdwq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3pdremkqd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vscbnbjc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rjmvrvnj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3obdqoptl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3bmtzlnxe.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qfuxelpu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3yjqayywo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nfszhuwt.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3uvbbicxe.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lrkkwlvu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ruydqymu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3taryrkcx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kgwdcvzk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3hsozkjjn.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ilvleoao.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3adxhtxmk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3clrhfcuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpkwingx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3glulxfkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbkwstxh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3mkgpjdpz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3tcfvigfq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3wprkqdlh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ydmevvfa.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3yeobaqub.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3wzcvvhri.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3bnlmbtuh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3qmezydpd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ucbxtasg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lkyaypss.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3gjsoppnp.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ixrseyms.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3lkcivrnm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3afvuodss.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ggniuzih.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3xcqlarfv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3hwcdgehi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3hdsxeimf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3jdebytux.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ftaiciei.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zxeqrils.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3tawmqpjh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3avljtjbb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3abgcuskv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3fymyshvq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3atflbsfd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3jktvueot.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ceotewdd.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3tusyqmcz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3alhctuei.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3bbtbjojk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hjygbadh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3jvjaxztz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3nrshqghx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3gjpzylak.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3inufdoao.html


<!-- 参考信息 -->