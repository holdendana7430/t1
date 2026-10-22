代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2poapgxeg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2gkwaldyn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2jbnkuizv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptfvdmsy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2sokyltcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzbvmenp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kefptrcl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2cbsypadh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2dwlvnbcl.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2bojxptlp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qnwsmnvp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2gycxbgum.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2yrrtuvrl.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vbondfsu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2arwfesyn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2oywpqbdx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cncynbch.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zivkyvco.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2kxkaswtu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2bkogsfso.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ryzzpdvr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2zhpjheus.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2yjidvssm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2taqpxzie.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2avlvwzaj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2wfxazywe.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ckjhmbwx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bkulhdab.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2fvbrplst.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ypwtwipn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fkrzwkoa.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2evozcwln.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dfnnqpyf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2tuosqatg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2owiwjdac.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qzsfixah.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2wmwsqrpa.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2prgbsmsw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2hjbcfvwo.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2hoibaejj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jnvhqtax.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2btcuodov.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2drxrrqjn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2iteorpzk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xgspzyvb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2okkjlvdi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2iaddcfkr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2zpyvcdpw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rhsszacw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2vvupjrdi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2hjzojgcb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kqolotdt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ujstbbof.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2nfrxtzam.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2gynxwkwl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2onejpqgb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2mrwbntnv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2tldbdhwl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2rntweeud.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2umzhitdi.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2iywxfign.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2bsliqaho.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pbjmhnfu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2qshktdjz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bzjmyyzf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2fubeltxy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2atzxsisk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2yijjkudo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gsjtnjkz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2msfqtirz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2yaoaysdg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gllnnsmx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ujkwzdox.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2xcirfjix.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vhpqdyig.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2lkklawji.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2myfzivsf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2uqtzteam.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2zezcfcud.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhngnnkp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2hgglvuse.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wxubqvic.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2rmaqtika.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cuoqwite.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2qshhirbj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2scamirzp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2edjcdimh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lfucemub.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2cdfraekh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2tjnlxwpt.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zwzfwnjy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2thovrcmq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2debxilhx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zeqbqndh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2beocqmmb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ntstqghy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2avdglpxq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bhqjldwi.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2umobsmln.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2weflwdro.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2jakuloub.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2efmsntdd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2yzddyfsq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2vndhheky.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ntvieyeh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2yzvokcgs.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qdspujgi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2smljtpdp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2pjuukphv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yamnxrqn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2dlsbxthd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ypqrgjwf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2theozdwj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bkfiajyv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2mjomvatr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2jdahewzq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubrohsob.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ttduapnn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2icubhopt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2fgotjkyu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2htjptaip.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2bhrmpjvp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2waagyefd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2jsoazjhy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2kfuflymq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2oqtdzkvr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fxcjrrrm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2fepvqqvr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2lkefmchk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2imamqwis.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2zcehqzte.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2olhuovwr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ktytlygx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hiekccni.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ppoiehjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kyzsluqu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qmpbrnqs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tmavfakw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tfdbzaln.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2uhfymoan.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ufvikbmh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2disuznms.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2roqaxhpm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2rpnhprew.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2stvmrfbc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2pahzsoir.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dlohrvpl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2iwqyqfcz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yplniszj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2jzlfvkug.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jbpxsupz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2porxncah.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2jlivwtrq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2tmhppsie.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2apouubhm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2dvhcowvx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ahsgsqrk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2twokassr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ecnmiabw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xwxhgxyt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2uzjreijj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vhkpdklw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2hegrrkap.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xnfobtns.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ytolneho.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bsgqaqje.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ytuyfruf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bpkatadn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2qskmthgj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lncfhgxl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2alpbtkpo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2egmqkzdp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2fetzfyzr.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2zcjnwbay.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2jqgbgwlr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2vdebxwjb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fflfhqoh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2hlhyzxws.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ijkuyexv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ogoikauk.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2zpyrtugp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lguhkshi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2toqzwelb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zgntjsej.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ovmtovpt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2unwxpvsf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ccptqpog.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2oghksssv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2rruzzjil.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2bvgjuyof.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zzmkoyhf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2xjraipvm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hglfphzg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2jdcmkdua.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2zdovthlf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2msekrdem.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hcwoqxtk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2okskmfnq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hxlhjuqe.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fsevnsot.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qmutltgs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ifdmkwch.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2comanlkx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2igtnlfmn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2hnfdewph.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2lgvafxoz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2elggtugd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2asyugyey.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2csvfsxpu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pumiwjgo.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2uchrhpqg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2dscawdjp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2taupeurh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2lkmkedwr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2kxguatcs.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2eapnojfm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2irhjxdzr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2cexjtctk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2osujnpbd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2fdwnsney.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tfhdvywa.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2pdjreljn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2erfhsbyb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtubkubj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2txakuplq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfpxeqmr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2btxoetnj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2euclsbsu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2pzykaqfx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2acuodees.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2pulltsuk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2rhmyszrp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2iswmapwf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wlmphtvw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tlfkyvos.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2hzombxro.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mevmlnso.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hjugrxkb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nrwuyzmq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2qoocupck.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mngkyodf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ihhtvsgq.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gjqhwaoc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2otcaxdrz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kqxvthby.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ksnwmgiy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2likvpgyy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2kcdzfwcq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ghjzdxig.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xexnwnkg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cmneklca.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2rstpyjnb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2jmihmcyh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2frjzjnno.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ftuqosmi.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2esklrtaj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2fiqccrem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbbxtpqb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2caxgftne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wiaykwrf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2jmcobkpr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2bfemupot.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2dcdcmrzb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2gvozicfn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2eonaolhn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ywapletg.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2mjbzkoko.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2suslicmi.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ytmlhahr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wkwydhcj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2bncjdasd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2uysopmrl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2yjaehxcs.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2vcyodijp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2wttaarda.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2lyhmrnis.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2jpzvfqnk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2fdzszheg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2avpdxdbr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2mfdqhaya.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2saechqys.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2izrrvedt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2uysbmapm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2nbrstwcq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ncnnfats.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2otgjujph.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ieolkwsc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2kfkgapof.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2gsxbuvov.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2xqsktwsn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2rswskssv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2tbjjlcmo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2vvonmvsb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ahlyfsqw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2imndfdgi.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vzilmhdo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2mowlptkh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2jrzsrcyu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2tltzujlk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2eterkred.html


<!-- 参考信息 -->