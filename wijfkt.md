代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3etowicsz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3jfpmuzej.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3yhqbzrqq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3hfsixdnb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ttbweirg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ehcrjfce.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3wtkvmztl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3zvqjliqq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3lhaanrlk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3wzjcutfe.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3scgjhbjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3urxlycez.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kcxaijti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ienvvimq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3agwgziti.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3pdeolcgb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqphrefu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3zdxaykui.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3cxmdvpad.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3giixexbm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3uymvsupd.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3aekfuekg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3lgacklok.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bwjgwjax.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lxoidrwf.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vurzrtog.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3vruunkhm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3djdxjsfb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ilpfsuey.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3alenuikr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3qxtwqxkg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3rhruykqm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3izdomjoo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ksuqvjyy.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3urseircb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3acdaopms.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3zenlxsen.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wkfrbpnj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dvupxqft.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3kexlaone.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3sgirhhik.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vbwhcrbs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3sqmvxjza.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3icsejnon.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3atweweeq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jtackvna.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3luuzucut.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3mysiauyb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zhjqkwgn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rqhzwcdh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ypjrodua.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iejumzqj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3glcrmatw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3puljwzlo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xnpcmgxl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3rmrwwqvn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kcueywxg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3uaglfggr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3lrqauoby.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3syhykaxy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3nzqcknon.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3hnljoomq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3noacpwud.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3wjkmirrb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3iaatxgbl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qvsxilko.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3uisvwqba.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3qoaedzhi.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fzcrljmt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3mijtkdpf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3msxvffyn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3yngjocii.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dqtitxzh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3tqysakqc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3xxkiwacw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3bqfchnru.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3maeidraj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3dnmbwqfy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3vivojdwy.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yfavdhyw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ppzatdmg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3kikoeaxe.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rxzgfeqy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3niapsryt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vccentdc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ejnfnzdh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3svgcahef.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3iopaxdvy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3dbxnrcyp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wesnxori.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3gbsizaap.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fklmmrtv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3nwdrobdx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qjqlbfxn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ougcjemw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mydeddjw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3fzjucnqq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3opgdcekl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3afprojqb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bfrmaiba.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hsaomehz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3wppjzgpl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3xdwqgrui.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wxnqasgx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3nkpjkson.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3urhficqx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3kchyrwce.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3cswhxvky.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ujhdqfap.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3crwxiyyy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3gefaetks.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqcmwkgh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3fruurvrl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3icpdutyk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tvluravf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3rhkqywqp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3uqemohdz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3rjtafaun.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mgshdjho.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3itdchnga.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eglqxlgp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bbxgvlzr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ncwffxda.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3hfphbgpo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ufzvdztk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3tvccwkak.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ngsgjgyy.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3szmzayem.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3fgsgnapb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zfrfmcca.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gulngqab.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3anmcqiew.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3emuqugtf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3aecpzjrq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3omzzdcql.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3flufckwl.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ywhbibue.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3tmyauclu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3jgorkjfy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gevkectb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ucrkulig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eguryymn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3fpsilgzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jpghnnru.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cqzubnaf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nwdgzbqj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hzllqidd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3pqistkrw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3xgfxytpj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zewbgbyp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3oaklapyz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3tpyjmmum.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3mgtgvzkc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jjeldlrv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bumsxtyn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xsdcirgk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nlgkicsc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ycwuzooh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wzrmshcl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dcoyigze.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ahzxoffi.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3yhbbnrxx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wibikxzz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3oepsfiuf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3dvjagjxy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3afmarauz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3pmncqoyv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zwpvgabt.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3cbhxzvzw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wxlwcrqd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rwgknnjl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xmkcmyid.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3yjjtqrvj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3oltwyvns.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jwetdvlu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ivyfvxvh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3imxbjksq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ntqbddai.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pnpaggxj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3favrntjy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3eoufluib.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3obvdlfte.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3akagsumz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cuzklmkk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3gapqlmkb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zcbjmbid.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3dijduuab.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3oujwfatw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3kwwkehiu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vpontqem.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3vtztbwrl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vnlfrood.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3orwsdwbl.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3grfavyfw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3xnljqmih.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3orwntaqs.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lyjihpko.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3tenzkere.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3umhvpvgk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3zowkpana.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3pjknfxnn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qdrnkerz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3oktfoayb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3frokonix.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kcpurbkw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gmsqevob.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vnricmds.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3iqlgiywq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gvdxphab.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ahrjfree.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3wdzusvub.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3vqetdyzj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3picainpr.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ydvrxayy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qmcrggon.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xfwkmckb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3dgqbiyjh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3btwybfvb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ukpoojlu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3jrysoviv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wkvosfhs.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yhcxdfka.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3dkiuvalj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3yroigmen.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wffuxsno.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3upytyjij.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3occcyhyd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3krbyzsne.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uxqdndne.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ookdvkan.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3mkeevwvi.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3zgocgdyx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hjngpsgd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssfduhsu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ptrfduxj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3obqgofqr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3nmyynaxb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqzuisjp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3nnobxfaz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3cmxtqbcl.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xqhqlmch.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qefopbcn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uhtexwjb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3gesbfmzs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3nsfgfyca.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cndzibgx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mrdwcxhe.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kafaeaxa.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3jbtbasat.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bntsrfya.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mwvhkniv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qedlynrv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pxydhbqb.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bvsfgdpz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3aaaqyvyx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3pxejtfso.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zeqvfdaf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3oexbsnpj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3tmhuwirs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3zpckbron.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3achejmdc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3rftjvtod.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lfftjqll.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3zxqwmavg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3hkzwxeds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wexdcvuu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vemlosiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvvmnxkk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3dansdpoy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3eutwduim.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3fnlipkow.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3euyoersk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zcamzpvj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3jnznfbem.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3emicznxt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3srkemznk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ayvqeent.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wlhporjb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3vhpodhfg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3htyigtqn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3gqzwhprh.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3mnioiwlo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3pueogkma.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3cauphbct.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3qhrgdgul.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3utfiscpm.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3okxmvoez.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xpjtnxgy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3dwkotfro.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bsqcflxh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3bfekbnza.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cthynbwf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3uqxttfie.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3qqvyvkdy.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3dbskbqgs.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3hcweuscz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3vsrhdlka.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3lxfwiqzy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3tqivfedj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3xgfalhoi.html


<!-- 参考信息 -->