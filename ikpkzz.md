代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3isjnobjx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3lvqzhcda.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3swrkpkdx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3fyofsxpq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3prvcnigz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3cymfgnlg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ekimqohf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3jtkkunbs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3hbicwtpi.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3drwemtul.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3vkadthxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkyviwro.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lzpwzvuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzmggbje.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iyptxhtw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3wdkewcay.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ltpuampm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ehokciqj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3jsllqdof.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zemkwpuu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3zwdjerby.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3fkrymoyv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xgiqmuuf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vlrljnft.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3cvncqbob.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3duoypmab.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3lygatdou.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rdfaefbk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3kimnrtvo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3dqpaqzpg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3kggvyrge.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3uvhkyouz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3knoroelb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3awbbiexi.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3sdzcligk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bxzrmgtq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3nrgjuvim.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3rfgowtmn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ypplnztk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3bgweszqx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3aghruwuu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3komggaqf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3hvftwfqe.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jcuboxlt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3kxfzbvis.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vkctyeyk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ieqyplqg.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3oeguwpjx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ihbcfbqq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qgwijngq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3yaloxull.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mbxjiudg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3bdwlkbby.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3yciakfvp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3skbwakbq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3tqjwbkun.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3thbiewem.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3lqiyvqvo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3qhtlgwnr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zsohffzt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3rwzsbdty.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pealseos.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3gchhrrwe.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3kvlqhyhf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3nktpgufh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3eliyjhfy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3kiaswkvq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3muajfinh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3zjjmqvoa.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3jiakjhhm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ubvkfcli.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ynidbcgc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3vvvzbnhd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3rrsqlled.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3sgvycrbs.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3qpqwnkuj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3xyvpirrd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vzgklhzz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3idbsbcle.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sptbutly.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3qpdctovo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3etiuclxw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3yfyqxfje.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ysabchrq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3darmdzog.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3hgqqvclt.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3mraghoju.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3jtyktkkj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3wrlaqmpx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hesawzmc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ajvougun.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fbzlxpre.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3rwlusuzv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3fboybbkg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3uvhjxxiy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rlsckyxd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ezazrtpl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3bgoemhhv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3kpgcopdj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3szagblbr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zuzzjzxb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3yvcdfsiu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ocfwzqhl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3fkezyicv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ldslnrno.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3koevpiut.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3yzpifzee.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3tjteivpo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3scpwsobo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3dmlszoyg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ewpkotso.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjzwzupd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mrzfeetw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3snvvdwks.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vmnopkgc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3vkxvwerj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3phnrxxes.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3tceysqrr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ixewnohy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3yciqzgnb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uwwzgrni.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pnyaynoc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ptkylpps.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3qgnhlvkj.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3abefsxhv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hiywxuot.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3xrolppho.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ljqmuvml.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pdyxfgvt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3adjrxfxl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yiajbfay.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3tkgecqms.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3cougyssk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jsacdsdn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3oaqdytxk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vqnfwjtx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hoguedzt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3jloabsog.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3fdefkdhp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3llcbycdi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3txcreije.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gastecen.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zsoneyhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pkwiyfpf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ptupsrfv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zjtwcmtf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3bnezqxyq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3cfkupfjw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3cymupyvb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fkbkjgjf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3uubdwbbk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3apypumvu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wptecprp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3eiraabin.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ssnbjjep.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gtswrvfh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zibaksne.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3shirtlhg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zrnoyzvy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kujomvmx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3foamkwvn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3rpocumbk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3sfiqdxdd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3cuhdxnuk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3fwrghesm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3vnqxspbb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3oaoupsqm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gsvpmwls.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3xiwaldks.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3tqtrrean.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3wvxomedq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vdrzlzwr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3riuianhf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3bgeurvpu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3shtzhidp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kxskronn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3lfldecbq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3weflivmi.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ekomerdm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3nigdezng.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ufmvmlkb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ttfuvzet.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3amnxrmwn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3tkpfphxj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jrcysnoi.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3krikrtwe.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3nnmloaqd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vcffkdfp.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jdkqtboo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lzxmwgzz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3siadzfyu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dxvqxfxr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3frtmiudf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zwfvqmwa.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3wrslligu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3pxbieajj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lxwvviel.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3juldrerj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jcmdfxme.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3drskmzia.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3udkwwffh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3xcjrgfkb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ryusxhfa.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ypmdhrph.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3afcbaulo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3riumzdqs.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3tddnrjui.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3djmdxbje.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3xnubwxql.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3bpnbkwye.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3meegqtyg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3bqkyogpj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3cnystmof.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qumwhvxk.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wqfvuwkt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3kubcvyaj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bdodxjdt.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3bumksyxr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rmhtznog.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3wtgfnjhv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3idvmlwvp.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3zrqyzotc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3hxcvrzth.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3extpcmti.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gttttkwp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jcydakdq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vbaonpyy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3yopydclh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fjbyozsl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lgnnibbt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3addiwhpu.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdtmpxig.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3aqhxtfff.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3luofcdxb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ywrjsjfa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ogkrsojt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3gtckucbf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3oyrjkagd.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3yigwbxof.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3pvlzrmrq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3yairufph.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuusentz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nsxiswvr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3jvslqvou.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3otbmhnvg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fzshixpp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kjvrzqtv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wkpoaolt.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nsymieer.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vddkilic.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jlvfeyab.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zwjifdtg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3akuurjtr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wmcttsro.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgsktjtw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3seujwewi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tlywirwo.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ezdahqoa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hdumlolf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3meteegmo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3axfasgjh.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gmmcybhb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qvsitiqs.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3oigfiffv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xeqpbbrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xonbiduy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fvagbnyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3siwksxxq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3wgiwajlz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3jaeikgbu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3fibdawwa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lopvyamw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vodjntxj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3eeoropgh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3hynnhmru.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ydinpqwx.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ywtbajpv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iolnvmxe.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3tglebttz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3qltrlhus.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ozvqytvc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3tgxwesku.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3zhtmfzrw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ewfhlrss.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3kmddwhvh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3zjdkknvu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3xgnhyyzv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3stuoddvz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ltympgwl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3sxlbezfq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3hcwupfdb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3pmwldsev.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3dyvrlqbo.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3qjitflal.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3efgxxtlv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3nflpybxs.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3hybrecpu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3bnzerypv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3itnnassl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3pfypaqrt.html


<!-- 参考信息 -->