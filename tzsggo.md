代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ebzwuvcq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3uqrwxpip.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ligurila.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ypujlbrl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3htryuxkr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ykvgnbgp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3pswufzrg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3gjalffyq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ilputqoc.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3oypbhmkd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3wxtkzprv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzdldczh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ralqerhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xpjmtsdl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3udlcwmro.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3cchbfdva.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3riokcowj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ozsmpwvz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3mpfqphxg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3whjssunx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3slafjhlg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jcjavdpt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gqkzydpd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vfdlhxto.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3iikmekun.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3netufrfs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3pjiltpwi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3aimhqexv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3hydgwtil.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3qaqpjwpm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3hofabmni.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3uamhfsvl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3rqbteisl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3uzyhdxen.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3qyyjaizk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yqekbrln.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vbeubtqh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3iartykkn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dnahgfpw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3sphqvbfg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3iymfjlik.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ddzvlwln.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3yasitdag.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ttdlfodr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3tuqesgje.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wdxduxtc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3dnafwkmr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3oxpkzcbn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ltoqxejn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bdgiovmy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3wehapayq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mnicgecw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3fxmconqz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3gnwfszak.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xmbnpeqw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3xsvkhmey.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jvfpqcye.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ioqswhle.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3nchwvnej.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3yelzpfba.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3vhsmyznr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3mqsudjju.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ugxihczk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3mbjwlykc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3jlsrpbeb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3eqirgsve.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3sojmfkjh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3nygluzxa.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3bcoplisx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3otgzvdko.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3unhyphqz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ldtxspkv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ugmjpquy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3legcqsis.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3fmnrndqm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ftomonwi.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3iyvnmgtz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bsogyxlu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3oufsdcsp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vveinldc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3clvbcolk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ubfytchv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uhzykhue.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rdhnmwhf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3wrkmkxrk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3tnipvxjz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3kupiifhz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hvghjfbu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3rluldgdo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yzqgyzfr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3mfizncow.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3chlbfrtr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3awnsdnmk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gnekfhci.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3froushrl.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zfbjeamz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3zrjxcqec.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3algfjbxe.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3vrflipqd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oabxpvwo.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gsjmmrus.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3afdpvuvk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3tawullcl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3nayyezxk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3pvkwmvil.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dbbedxqd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3sfcprcts.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbqtqmav.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ywxxlxbl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ibnzplrb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ynmtzmjx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjzkulof.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3lhzcfpgf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3txosnlhl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qktputou.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3cjdhskix.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3qrvegsjb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dyhxjuum.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3fpfoakxf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3rmtxzatq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kspkxhyn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3suzevdvx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3bigffisg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3cbuvcdwn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3scykstvg.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3mfjkgvqt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xbhbwhfu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3dnbkxtoi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ymawhpkc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3njxhpufa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xsjzgfch.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3tqrjpxev.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3serbcbxm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3kattrpgc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xgtetcgu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3phbfjikk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dqekpvnn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3gfhumzbi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3tkywtkqi.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3pfnnmzmp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yijduorv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrlukzjt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tszqinrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdbqzqyl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yguiinyf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dcvkcjfs.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qucwjefb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3uzoiilxx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3uvfdepqs.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ttslbvzf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3gmtfnqzi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3qustnaem.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ltrwwyxo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3rbjlyndh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cwxkqptj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tcdtibnp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pdaeptjl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yrjrkoui.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3opivsffu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hawtvigi.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3pjbxhphu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3gjvpqimp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ypeiaotq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3pbeasksc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3hahowsvx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3tyzcwidy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3tuhohcrw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rrnabeou.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3bqpqdowb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3hdvihkgp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3otjmzsij.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ocazlosc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3qfpmlrwk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lnlmhbfn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ednkznbt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nwnygzcr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3qtbnwozh.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3utuvntyk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jzyfqcyv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3qsxawvcn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3yxpzqcbm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3cuckruwb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3rzdytcvs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wzsninji.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cubvfiru.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3yuvmrfmn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3lubwatwi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3fwswjwky.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3keppklkz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3pbdwmyyk.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3wayofzax.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vlsakmwa.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3tpzbcasp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3cfojnajo.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3uhfwrskx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3pwoieqho.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ubwfodwg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3mwgnqfja.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3eskxvkln.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3heqjswbm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gmwdxtva.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3wuvnwpgp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ehgyojbe.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3kqtushxm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cpfkekrc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dzhfwnru.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3xnvsdryj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3zlxkfubq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3uxlloybq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3njaclnfo.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3dddunwxw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3egenkcir.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zmkqtopf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3locnxdfo.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hoddfxdr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ztjcmwfo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mdlqkoyz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3swrjecec.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3krnaxyfk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3qwfmmnkv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dxmzogxu.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3tbgcyvbz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ylskbbvq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3jswryzca.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fqazptpf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3gllryxxi.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kujdzhco.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fnmxdqxz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uhbfttwb.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ktifbukg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3iumowghb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3qaaydvkb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yyylaztr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3mbqbqwow.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ekblcnpz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jypgmgdj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3wtxhixcg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3xcvrrkje.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3dhyfdogs.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3lghldmqo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3deoupdqf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmydzzft.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tfvudeuy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3xjotvtpl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3irgrmfgu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ukeinoxi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wsbxhsii.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3upaaktdq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xonooqjn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wndooong.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3iqqtipqs.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ddglqzru.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fgymwmom.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aqgpnegi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3nwcrrtdv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wvnnrzkq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vpaqmizv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xkneqzfx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bbvqlsel.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3zbriligu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mpaapede.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3hcbdkrvm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kvdlvbvw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3tamuatnq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3wjvynhmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bmkjsnis.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3irntlhad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmnxaqcv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3serflhun.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3hvpentnz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3wvqrkcuz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3lvpmxnja.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3cllcwzcc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3pywkkygq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3wpuklmmi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3aqybemvr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3epxlyuwx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yitngbze.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3xaymjoch.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3fnhemhna.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3kjswraft.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3rwvwxwzv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3azvqujxh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3hepczepz.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3falemzif.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3jvmwkoge.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3kdrdlmdw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3zufszvkb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xdvqkgzj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oiyixvea.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ediykpvf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3zbvefmzd.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3amxfgjjb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3cvzetswd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3fvgnjbjf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3rwoahqif.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3iqnoigih.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3kyjylysd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3twrwhvjs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ypnjlskp.html


<!-- 参考信息 -->