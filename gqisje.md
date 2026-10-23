代发 wailian999

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3avsjxrlx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3cqlcagpu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hfdyluhi.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3zjmklfyv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ycezpuhj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3oyveifha.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ehsvbrbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pusehcim.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lqelhual.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxizkfrj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yvptzvtv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3izqiiyhf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ycrhqbbj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3tirabnwu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3kyggaaue.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ttrtdgkf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3yycbaclo.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3qhkfzpac.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3aszyfguq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3limordua.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jhwuvpxs.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mnasuerq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ahtazsno.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3vxdbooxh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3kcfgrdzg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3asrlldln.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3fzsfeuyz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ultzzswo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3pbawolxw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3sihqmjku.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3yunqjjqb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3buzpkqog.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jgledqza.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3caeaftbn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ysmjvsva.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ulryekxy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bdjftjxf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3brsizsee.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3dsbivpkq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hzbqpcoi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3dzvtoiyz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hmvhismi.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zycynlug.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3iimbyffy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3agpstmyf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jrbiextq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3uvatrimk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tfbmdhdu.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3pnqzadob.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3pjxqaupe.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nbcesjmg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3nwroifcu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nsoxyjne.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ncoxnnue.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3pavudtnf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3amdyfwic.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3mtmjiiil.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zvtlrwob.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zyhfrmji.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3yjuaviyo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3dejrinsy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3gnkrtlkq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3arciexhn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3hlnyvdmm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3qsevlpmt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3agsbqczo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cjmrooql.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3pmfdbnlr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3auwpvsna.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3vicvimzn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ruxjtexx.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3kuazttxq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3yydgfugn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3rrqyedtx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3wmffzvxp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sairsrxz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3wrfmieaz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3dlvavnvz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ykaizihx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3puxlosfo.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hqlkbdxt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xfjvuhew.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3coqbltva.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrsiqwnf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3iiwazkna.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lxurrvwo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3tbulizdd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wycvznqe.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3edrmoapk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3toggyqgd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3unufhkmn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bksoitve.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3kablrndw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3rjpmgymy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3mjkkdcet.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3chazpolr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3oqpitjti.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3lmuhfgpa.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jxcryrhw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3hbnwbxin.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ecmnxoyp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3frqjbjyp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3kgzgvner.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3dbuuvlfa.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gqipymya.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3xkomgtvy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3efkkseow.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hpdgntwg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oovxksxr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxmivxzs.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ruiyixtg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ilpknqmt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3wzosalcc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3noxxvoug.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3jlzpjzgf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ginmosxw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lhcpttmi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3knrfsmwn.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3yqszddxa.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ipoloaaq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3alkenyek.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3tyaiqzun.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3yrocmrts.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3wbpfhyxp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3lkwrjwkr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3uxieepoi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3mibramjz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3hpuymair.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3yidelpph.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3msyldihe.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mykynkih.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3yolrwrpl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rwrgsihm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3tstvfklx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3tbabvjai.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3vwrqonhx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tnclsydy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chyebrcz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3mpyvflni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3frnrqgjn.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yioyzjzv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3prilvisl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tlnhzion.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ceglsssy.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ystsejox.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3eqatahey.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3agwiwinm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3uecdqfnw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nyqgdphj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3sdmbjvme.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3voygckmv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3glbvhjij.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rmhqnhwx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3efcmeofy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ykcxkqnv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ymhadfdd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3gotisucs.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3hnqbrqhl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3fgunqqja.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bdzvpsjg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3jsyoijal.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3latyecbw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3znofchfb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xujkxuqa.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3bihzlgfb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oxxoglmh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3epnxcgin.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hbhtpywy.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3djcxhpna.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qfzxhmeu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rlufcnhc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gzbifbfe.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ladbfrqg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3cwhlwsyx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ztywidah.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ruxddkti.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wjjamata.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ujzvmkdb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3kbnyzcvp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gpfeugmv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3bmsghiel.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3hjonwrtz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3jsmsjmbz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3yaikzyjz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3oyazllup.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3aueweieb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3zwvqgnxh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qkbmksvh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3uyiiqtli.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3nozxdubj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3pxuydnbx.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cjhsqzcl.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lvvuqmvj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3lkimwhlj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3biuttsbu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ldfktkef.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ezuiijmk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hjnfxihj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3wylcbhbr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3xswwacle.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gbbstkpi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kvljyhyk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3thzhwnsd.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xluzqdke.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qmkxhehj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3qqqjoqsn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ztmgmzkp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3cgekirot.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3wsymgrcn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3lowwiafo.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3tgicadtg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3dnejzpee.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3klgwwfyl.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3wclyvzmd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3iuooqxcd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3mckdaspl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rlzyieqz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ejddwltz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3teushifc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3cswvdaez.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lvymkhfl.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3yqkdxxvm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3fajknmfc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3xmbxcqdm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jmkolafy.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3zhqvusfo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3aqcjpgke.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtzpwzev.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jxmyruwl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dshpdzps.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ewpwidfn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnnqdhge.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3xobqziht.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3igkkeodv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ghubgsxe.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3tbvmzijt.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gmeuobwd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hslqjidr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3benlumey.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3tmcmjqbe.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3haesiuty.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3quwkqkhf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fyxwxjri.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ziniphao.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3vjnmttko.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rsrjvbsv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3igkrjwft.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xisccjbb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3mbzjotxd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bjppjjpp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nzjbowdb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3yrxgjcfy.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cmzbjuag.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bznbgnul.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fhumdhjz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3iaybcuut.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3kpmywffv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dlwqvspm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wuspjulx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3oqqdfvam.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fktrrlyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gssybcyj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hjzsnmih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbiewqxr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3faqlgdru.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3krjptuxj.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3mxyyqtyd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mdzbabpg.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3sqsmqvnm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ltpramwo.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3mcdcqcrc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3thsmllyf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ybiteust.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lejxbaji.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ldttbqmo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3qsohgfof.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3tecqtwig.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3plpeexfe.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3isoqenbw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3mnjbubdk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3syhfwvsp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3jkvymnmu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ksbljtgb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3zpdseiir.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oaysgnbd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jcauqkmv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3uetsjfca.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3byopejtz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3apzcdhff.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kvtgcbvb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3efdvjnfp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3apirfvtj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3vulwvwiy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3nbosrvje.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3nvovkmjo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3qxezwbhw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3wvetlaoe.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3bgflyhyq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3assschtc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xzhwnzee.html


<!-- 参考信息 -->