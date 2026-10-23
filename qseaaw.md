代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3sndmpznt.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3dfxaatve.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bzkjqqxx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3kwrnukvn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3odwijjka.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3fpxiwtvr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lgfntvan.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qvjqjnpt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3nywyddxj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3rzfvkayp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ymokpqxd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3tquhseea.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3xtsiqidt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3sooyqpbl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3qpdsnhlq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3aiqwqohu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3achdsnrn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jfwqrlsg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3jqkqyzon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgdfkiou.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3dsuolosv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cehvqwnm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3phtpczui.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xkqttoon.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymqyvkue.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3cufhjeqs.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3dyotxxsm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3gyexjzjz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3gffqtwue.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3csejirmf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3isfnkvpn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rxggwpfy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3tcskanzc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hxnvmynh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ihyxcsbq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jrzfddwc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3lswmyqur.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3xvvqepfo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3qheowtvq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3qylbcugg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3bcvmetoh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3cgyldvos.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3psukyybu.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tsldziyq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3gpzrixqz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ikqmeanl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dulkmxop.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3jgcozjer.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rtvtcduv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3mnppwtmz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3perliomg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3viekkyot.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3joolmbhs.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3nihknvbe.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3dimkycel.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3hsdgmtov.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jsyhfxwn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bbvournf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3tbapllph.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3udihatod.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3plhjjvky.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3oonfxznr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tldhrknt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3wpippyki.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gmkbevjp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3reidncwa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3uunngayd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ewbdjqjh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3isdfgrmk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mnqquinu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3dntzngai.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3foubnwly.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3weialriu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jrlhadke.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3yiqwjpyz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3kckazunb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hbviwnrk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3zdyjutjq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hxxoifeu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3lyoskcxd.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3xifiqrcb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3invkzygk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3zizykdcg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3tepsilfy.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gwaewacd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3bmjjvrcp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3rkweluxw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ltpicgkb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3qdliirfi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3akziyicq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rxlmypjg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hbhutbal.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3yijmifyp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kwuakpcp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3risdvrlt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xizsfyxp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ieqqespr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lipztoal.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qkhrldyc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tlvbgqjh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3fyjflunk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3scbvecnq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ltudbgqk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vvotvxqz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ksuizeef.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3pgvwzmeb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3qohaleuf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rrqsymjo.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sumeudot.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3uihzysha.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3upjdqzff.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lcskskub.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3khcyeqeu.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3hagazmjz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xwshgqet.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvnvfmkp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3rkesgxve.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3nrmqbblo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3vwcdybwa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jmkhccjc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iypmwlmf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3hringyvz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tfmmstew.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3nashfseo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ndvgxpal.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3oleqrchx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3smravgyo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3hqopmzqn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ogmxnghk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ytzvvyho.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ivujdjcl.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3zgdpausw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdkioesn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3nnflmrel.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3hcnjvniq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3vfqomlca.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3yyrxpsje.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3luttnzub.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kkxgiguy.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3zeqslenc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3bphzzszn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3joprbjdc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3mxxgpyjj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3lkppvtur.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3npcbtvwe.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3bpugzana.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ifklkvie.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3sqpbkpyh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xfhfwnrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cppodixh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qdbzhnjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxtbjpnb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ilyexmxm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qxtmzohx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ruizazdi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3rhngejln.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3zsygckhm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yvmmnrfr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3leqzivoh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3nlapeaet.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3aiuximhg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3pqfzwxvy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gjqnbtko.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3agfqsxmw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wiuhqoia.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3phjkmbjw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ynpyszcc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jhbxxkco.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3bhlctmaq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3bobufybc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3sonrntft.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3atqpcjdm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3tqsgpfol.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3swovriuh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3bbsvumww.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dcnusaqi.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3fcxiuoyz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3temlevsu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3omgfcpgf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3caujwrkh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zrtipltz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3fggaxlhk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xtkfgpxe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ziljkveo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3lmpksffm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tzjdvuku.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kcsrdvwf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3orgqsvvn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ggmhpubf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3bblvmhdv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dqntpnxr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3upkqiagf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dtpxhgrv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3hyioyhho.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3vayfglcs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3mbfphcsy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uhuwxvtz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ghuovoyq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xponzgwz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3whgogyqf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3sbnymleq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3lpsmmcwp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3nrvfajnn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mcjlptgf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3mpdmaxsi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3eirrrldp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3aqmrqltd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3aovebncx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3olcvedjm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3jlcrgwdo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3rfuzylnj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kdexjogc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gjfiltej.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dcttowls.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3xwwxtios.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3hyexyicw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3nzxjurpu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3qdlnoidi.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3kbgxgzzf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3tdtzaufs.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3lramfdhe.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bpdzpbct.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3cvqlyonm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3nqwetywd.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wxtbjugs.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ncwtqorh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ckwlczil.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3xehyjqiy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3udsgsnua.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3josiwuqo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3bqbstmql.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3eyamtqnz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oatgimby.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3fztaelht.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3plucirfv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3uiakacfl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gtvocpzg.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3vfathtyh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gctqhuqk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyujarnk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3gdnzcujn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3anuobiqq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3oxoscaum.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgemnoxs.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3sokmxgrb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3jjducyfy.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3wclxujok.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3epksdddq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bgqtddju.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3admfqjrw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sbchhcru.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3razsdwgj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3oelliqjp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cibhnivx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bysinlaf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3lyerixfq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pjpzpjqq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zyaaqrpt.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3uruvooux.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gyzwhpto.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wbmgnatd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3buzgkjgt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3rybzxjhs.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3gjmtusjx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3typsdhbb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ahjwxxiw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mhiqcfum.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3gqfujxbr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3rbaxflli.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zvmhhrki.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3sqdiqdmt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3fschrewr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3wqkvutxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oeuyrbzr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dcipnjar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rywjhkhr.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3kqlokpnl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3gubflbte.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3jaarzxsp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cgjvizer.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nvmosizc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3scwqwqzn.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3hzelfrjf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3neqewdnx.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ontkkxod.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wdswpdmd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3aqngggyk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3eyviiahq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3vtmbvthc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3tbwynlcl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3gmvaxhzo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3shvltfwd.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3mjuvfayr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3vzismbny.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3aolgggbg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ewcfbdaj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3vhosmwup.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3cuaplxmh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ypntizoh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jrizgfpz.html


<!-- 参考信息 -->