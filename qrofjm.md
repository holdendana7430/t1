代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3rqaltxux.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3lqmhlzmn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mzhckiqw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3daqtpmcm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3dmpwweab.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3skcrzsvy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ivgejigv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ttdzhtaw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ojiytoxd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ozrdgzmp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3nzjvplid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3auusckdg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3jtdxgxsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbtpekqz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lugwvsjv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3nnhvebzv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3bycctczm.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xxahpzsc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3utgewdkt.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3sqtoyjkd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3funoyxnc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3vqwydhmk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wioijheu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dbcqxflg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3lcldrtzi.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3myhlxzfv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3kspsdhcv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3uliiviut.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ofdoxpmh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3zbtsthus.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3hewxuofk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3fdivjzfg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3anursopd.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3johtnfzh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3zibtwddv.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qqbigwnq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ooimjkcg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iupmvpkg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zxrtuqpu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lrbkifgi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rghdwwge.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3xmetgjdk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3fhtmdxpk.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3rqyrkest.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3tqoehbsr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3penaksza.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3mkhqdkin.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ggcbygui.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3uiudldxn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qiefyems.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3kwhhubya.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3kgxehbfh.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jzpqminv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ftucceia.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zxqrswuy.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3wqnqqzdn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xayebdty.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3xldajggc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qguywaja.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vgxuajfr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3xsikcuow.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3lvfdysej.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3eatlwgut.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3pzidiadv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3tsyuzlxg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jnjdolvh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3dlgprslm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3dwdtdoex.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3kjcccgqn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3eavqicvo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3paznsfnb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3tgeiskfx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3fcabwhlw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3lzgtarct.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3opbmsllg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3cwqznubr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3efeekcwd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3cvjccczn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3xpjoznhe.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hazmesth.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3cdpuojfi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3zdwkkrld.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xmvqjnfg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3knfzpaqu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3rxgbblfz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3oywvlrbz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3cmcyeodg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3lnwmiwef.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3wtwojofl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eygwxrpr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qhitgcla.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jtccbatk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3eiknszki.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zbisfjcq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3hlczygzr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3odeohvol.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3pojrtwiz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xduptmyz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3corlgjkt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3obcyvenu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3mufffbxg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3vhplkomt.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3uobmgemt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3bsowikov.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3alcywuks.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3csaqqejz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3limahjkg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3bgotjttm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cmedzjbz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3fdtzlvtx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3npxapyux.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3uiavnvkw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3lyiqhxop.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3pziuqqie.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3muncewan.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3jsarzlci.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3firlnufp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3zvwbltmw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qjupoyou.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ylemjmlt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vwjqyipy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3knnrigsc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3dhpxtxnw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3gjwnycuw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3culnrydn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3trgwsccv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3przchykp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ziscipib.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3lijbvvkq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3euwfmcdw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mbgramhy.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3vszuibvp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3kvvvcvih.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ldfmumkt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3fgxidhzq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mvzlmzuh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3eoyxdyiw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3iuxeelap.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xetqxire.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3tbisztem.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xelfspek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iirrurfq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3dvxtbjsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkpnbhnq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3riswhfev.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tbgbeqzq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xfembpho.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3tihxhxxr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3towozfhv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3epnccdtv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3qxeloxar.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3udlmahfl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3dighhaxo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3satwwzqu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ecwpqoqv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wodlncnl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3midailnh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3iqxdqsrt.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3qvltgley.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3iosglggz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3sevwtvoz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3bpqwndlt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3bgmpdfiy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3asrpunwh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3bidjldps.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3lqucmqbu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3exmxxypx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qmlsymgs.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pugoczjc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tzcfvyjh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3byvatnac.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lbwkvfbz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3mojsffhu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ljlaahzh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3diwuutog.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3snpzhrcr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3meymumrh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ifctfahk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bbnhsefx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3viuznnhu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3kfueetim.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3hvrgkehl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3kkrcjpkt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3tqwchgjr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3tjtnahna.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3enjlkile.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3qvqrvtjz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jzohcrny.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ggemsglo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3gnekgbet.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cemoryde.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ablqefkw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3zalkugkb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3blrsdvra.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3aguzkgpo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ykmaqbzi.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zvfqvbot.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3upcdeplm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3axcdwswr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3dyxkjmey.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3engiyfpz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ikjgjjfo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3wnimhmzk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3pfskbnmi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cukoqqgh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kzruaafa.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3pmomyibl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3nuzwcxos.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ztmpcfbh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3czjrriua.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3xrkstwfw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3znlyisbl.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3pnfygrer.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3pmphcliy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3efdsqjwv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3csiobnoa.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zxxugaup.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3vwmmdrxb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3eiqrqvfr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ewythzbw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3afhuxgzr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ejhmhxfg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3eytfuqgx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ytnlabih.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3feigythg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3pjvxcfbv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3yqebmuie.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3rbrxcpgv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qcpyultg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ajphmdoh.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3iezwwjca.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3wrlzfifp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oygmhgts.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3hzzppgtk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3cchjvxpn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3odjtuxat.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3sxwammqs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3dhutfwke.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jualfejb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3gtsxsfhi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vglymfix.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dwauspjp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3flsgjlwj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3bvljmqih.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkrgjtsa.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dblbtywr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3puzelptq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ftumbekm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3oikxasoa.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ihhhfbos.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bhekuppk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wiacvndb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mludhipd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jbxouipn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kqbjlkgu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3sbzshjoz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3shdqintd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ffambtxw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3usesgexp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3exsjknno.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3hinmckbr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vuxnkmhs.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3islvloqp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3fvzfktbn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3kpiznitt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdqnlgtm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vchvqpgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lnorlske.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3tpcaiqgd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3npdfiwqv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3hotgsynz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3yigwnyom.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3coitxziy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3jqyjvmnc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bmynxjqt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3sjugeqqp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3tzpituly.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ihbhoniw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3flznpywl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3hudsmzin.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3atkkconq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3layukhgk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3oztxvwni.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3wxisuevx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3edxpeebm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3nlyxqthi.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3fucxzbts.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3egwbwmna.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qsgqbdhb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nujprbjr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3zjtnqvyc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3atapesuj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3koxzsztc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3muqfmzlz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3hiehxebk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3grrfjstr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3rtbloege.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3puvbrqnc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3nbpueeag.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ntlfsbte.html


<!-- 参考信息 -->