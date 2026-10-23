代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3dcmvzrdk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3bihukccr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3utmkpzjm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dnfucrhu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3xddqqucf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3lhvfqsgu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3vdudsedm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ggpkndgd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3voutkgou.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3zmqyxkyk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3vfiecluh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hljyitak.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pdvbpuxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwmvnwtp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nwraswej.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ljgtuxej.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhgdvxwh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wpyfgliy.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3aufrsqvz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3cyhbuhkn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3higkqwve.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3qytuenmf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nglpgjnl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dbqelwcs.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3uibtacwe.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3anslnggz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3kadbrlhj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3hhgqkhcj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3mbgrayjz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3sgtptidh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3iddmpsgg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3icdgeyur.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ioflsojq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3lrzypndc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3birgjkkl.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gebntehv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3yqovwcup.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3febygqix.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bogajykm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3xrzvijyn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yzzxixkj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3qindcjqy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3dkdorueq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hxjhzmmq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3wqugujqz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3rupeyhyp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3fyhjmcxl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3bptrchnj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fgcmqrfg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ifhfkodb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3mjlrjwln.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ljptdkuf.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3deuuxfac.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3tsbvpdka.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xapzrjio.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3eqnmwfzt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3oavvqhuv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3jfjbdsmj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3gnhaivvw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xfwpgdlr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3egzqcavb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3jnriwbaa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3syhfirae.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3rgtpewna.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3kanxjenu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3whbsdahx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3hhrxzgzi.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3myqjvvgv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3prqysuvo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qbjogata.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hktuhlif.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3xvwhyfdk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3cqpcqhlu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3cxhvozan.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3zkchajrl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3fjgdlyfm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nbhotena.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vfjqvscy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3xegxoxkr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nxxzuvsg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3zqawbril.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3moibjifr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qubxhedg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3lreoczck.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ydmmmwii.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wpufpytn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3horknzaw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnwxilio.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3wdwpcarc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3whwqihzr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ipottkjb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ojkeswne.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ellhbqqq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ffnsrzwy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3quwlwyof.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qqrzeesx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3qnasexsu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3dzibstnr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ldgbrwli.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qnmcstic.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pohigljb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3xsucfxhk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3crioppfw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3yirsnega.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3beucymrw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3oolelvbi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3prpoatsl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3vwqahyna.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3iinfpghi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3vwjzxchk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3cpxayzkc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hbvxjtyg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cxdpxvln.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3fzfpvsrt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fgcnznrl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3hdtezbug.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3rtxypqzb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qlkudppm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3vaqbogwn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3bseimdar.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3btagthpr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3xjltbyzd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3dnicnkro.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3cwpyuqng.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3djyrltgx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3djolgkvj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3kqnrnxgb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3jfapblgx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ldeafjcj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xsgttgdi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hwymvthy.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3jsnbfyen.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ahqbrfkn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3tatakhip.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3zebqiily.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3sielxizv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dzwhmiaj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3hcfuztif.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ohbpbrgf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3uxeukyhl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yiekzpyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmxouflc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qbwwtjzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtrvwvnd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bmehbrub.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3svppicti.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ffvcsjlv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3gjwsdtne.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ryhlteut.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vozcloqc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3pszhwfwi.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3lmfzxqsp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qsmpelxa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3mflwdcky.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cbehqljh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xsvgixfi.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bfjusigs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fxwkydjn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fudeqaob.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3dauwevds.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3rvldyjhu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vherzljx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hchoycjb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3aigydwpm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3rxyirtko.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3pebgsqqo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3oyykjhqu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kaaandgc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ahqbvvod.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zcugacgt.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gquxwkgk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yxjikfsi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rpblayzv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ddwtgylr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ajjdagii.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nqriqwkt.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ijfzscac.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tjefaqef.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lddigdhv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3nuvrxhwe.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3iuhaltba.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3tyvbqtlh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3qusykvhr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3imgkdmed.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ozbktzig.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3gdgzkaoe.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3yrowlmvp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3oenvshjm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3lyxpfupo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3phitrozk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wwkiqzpb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3joicycsn.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3qpnkvyhg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3xcskbxwc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3whtjmtpf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tcgkuqmm.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3elzugwwf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3itkkthjk.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3izknccwi.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ugiiooqz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3norrcyrv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qtqgifwe.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3bchfoeig.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kihwccqb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bbswtaaw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cegreogw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jkbkjsjx.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rvrldrcn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3rwdsoslw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fbbcozxz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3irzpberx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3caykxlhb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3tewsmayo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3tuwcxuit.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3spxndscb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3txlzkaay.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ssndpvuh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3bjfmmpob.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3zucgozjz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3gmzrhrxl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uvhvjwzc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ingaawvb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3oxxeupzl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3weysyzcf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3myfbrzba.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3lfwcsomc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3txlzlvbt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3zgdacvdx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lbmasxdl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3wwtxsvrt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3wqeaeoox.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3tcrlgvqp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3gsmualkq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3grbvcbaz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3czbicusa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufhjbgaq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ltrzfwxr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3rxlkkgqe.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jxfxixlr.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3dbzrchmr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3xacqxvzk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3njokofks.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lbwipere.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3oxhqjjfu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xiojyybi.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dshaymil.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oqzqqcic.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3sjlkrzdv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3egelqqhv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3advlogfn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ytszustj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fjewykxr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zdfvleav.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vimsnsqk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3sbjscsgt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3gryvtutx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3bmkicouv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kdsqumco.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3irupplnc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3erltuqry.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3hhcqqvxb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vxynjxxu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qscemorg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3yqfmwato.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3kvnjxlcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kmyrfxam.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3jinkfmsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrvzersr.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3yfixrdho.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3vklsdbhv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3mawnuurz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3oclzukgt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ouomcowv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3dczotyap.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3muudtyez.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3hgcwircx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3vdgixewf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3diuwajvb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3uakzikzb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3pvqelijx.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ryizipfk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3zzxspoqz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3okvirmnz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ejiffmpo.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3hjkbszmi.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3uhmkxzgt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3atwoqkpo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ggavuttv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3rzwrhaxa.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3obilavcx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3szgdnwrs.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3zzggguzf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3toenidmb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3lxwicygf.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3hsadypvs.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3yeufhhye.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3nghqskrj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3snmvdnau.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ahwbddgo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3illhojpp.html


<!-- 参考信息 -->