代发 wailian999

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3uufssjqj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3yecqghfb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3dygsxxrd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3utxqbttn.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ugdqcnco.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ymqvsnmt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3bkbbjgwx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3cumqecmo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3hsekknlk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3pusfjzcl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3pchoinjg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3snwloupd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3kexqmenb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3fqgcslxu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3sfmpgtdb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hbfztsog.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3bdymmpyj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gddpgpew.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3snuisbrf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3daiizoqm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kacsjtty.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3bldyvjld.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3exsqpahn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3gwkeedjj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3kbhrxnkm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3elpqgikw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3tldvbgin.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ojhplvyq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zcrpsrhm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ocnpvsha.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3uieipnkk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ecgiklor.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3wwwpfszw.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3dvchoxgh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pekriwzs.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3yxmtqndc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3iksihcbx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dteuyvli.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3sftdejyk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3igtykvek.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3aicidlis.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3dfelntxl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mlnztsfr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3cxzszqnf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3nzwwuppg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3erobvcfz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3phfqbjwe.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3rnmgxaiy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3amxgzjrr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3gwqhfors.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ywocdwcu.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3acjypaly.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zwnvptuk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3pcoxaolz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3cxnjoabs.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3awqndccj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zrcfmopa.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3aqmggsoo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3xqbrfjri.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wcdjuvmd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3eseqpwns.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3yjhqwzgy.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hqfdbsxl.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vydmeojx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3pozpzrfs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3vqpgmzby.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qnchriuu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywzlpdia.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ewrwlfzu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rsqekjmr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ueltrmyb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tvudtmtk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3rtsqgmqr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3nrtfozog.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ncceggsn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nzsofuct.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3svqvylnl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3njutwdui.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ocfhsdfv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sabwaaqz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3paesdhyd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3qthtlfsk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3vplwpeuj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3zpyjsbfo.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3jltfmfeh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3cjuisxnj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3vjrtaspb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqaxddrq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3upfykypz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3galugobg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3zdrkfmwr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hetngqtx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uloirhel.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgdfxaxf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qrzdmtnr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3mzwuueba.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vszocxox.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3uevsvhgn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3joyrqnyc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3lytofdcn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lkrxtmrh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3bopqnhpt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3dxvmlhjt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bueqwmbi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndvvmphp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3djodktoh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3uwpjcsna.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3uhgvxjcp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vdfedixo.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3eucdfjin.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3nmucqrvj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3nlcphtow.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ckirimyq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3zbthplqi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3miryjvik.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nzhigkph.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dvunxksk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3jrgvghxt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3huatdalb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ohmvflyd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qqomfwgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfdumfgs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rosugfye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ocvlvsmo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nahuuemw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rutyaegf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3tvqwgvmj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3lznsesgf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3gzltnnvz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vgusaoid.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3uuspyqnt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qujfuyhi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3htoponxp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3jahisrlk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3aqlqgopr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3czhppnbq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wphpzqlg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3usqsjxmf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3qcqbgluz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ejhhnkad.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3twikigjh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3kaqzzwtp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kvnxwzic.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3mxwcogem.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3adorhnku.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3prbvdtzn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3wrycvukn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qtaxchfr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3qvtcfydw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nwgnedyv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3joqaiygg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xhupziel.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3pyhqmcme.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3yjuqqdno.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bxkkvphi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3oirlffsz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3pwowoufs.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hzarharh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3efgzvpwq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3eahtxcfo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fbmgvnzj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3rrwufobm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3nkwdejru.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ipbsmovs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qlmvevwg.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ikmnebza.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3yubasidp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3amxnptlh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dfccicrt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3srkdthrl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wgihbgyq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qzsijimd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3nytfxkou.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3wtwksnbb.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3aqkehqfx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3obwlswzp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3iiwmuvxs.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ujhgeawc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ctsorjfh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3gtzkleuz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3icbecclg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3acjfhuyh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3eacqovcw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ujstowfv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wcndlwca.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3oenrklpl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3swsnqhuv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3uyarbxcw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3dnfmtzio.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ttuletxf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3jdvrqnxv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3giozbtmu.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3crvsbakw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3anibzucb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ojpyrlzl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3udsboeho.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3idfxepqe.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3nowhrlze.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3qdpzjqoj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3skoljhmo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fgccbhbh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3dojjqqcu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3jhekcwym.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3xvsjraak.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qeytsrel.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fjfglrsm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3mtxdounj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jpnsjvnr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eozvzkkf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3dtlvrffx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3hkbdohmh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbrknbbe.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3utqfcvnp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqwavkpn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3sxdjovuf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzsqvwun.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3onltvvao.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3hffehqcl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3iniezter.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3hozllawb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3fsxxqmsh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jfdbvjev.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3awiazvsk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3mjppfqcl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3imkllxeo.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oumvaeip.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gpbwttor.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3wjxltxmo.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3sgcbkgzh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3myaaxnkh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kbjxqtay.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hujzfelr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ekcwmjqx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ohlzjbid.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zgpvbtsf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ejjmyqvy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3eovxjzjl.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ihrzeumu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zcbnnoht.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3kiopajtk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3eorhntgf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3nondqxrs.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3urstnibc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3lupufxmr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3unklxocj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzlisimc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3plevbsch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3duspsjjz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3khcovlxx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3tdumcyqw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3layszikp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3bwdnwcdq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ngzaoygm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3rdwxtbvm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3cduehcry.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3udonbcay.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3pfmaauqp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tmcsjzez.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3emxriusj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3uwvbctgh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3xxiqcycr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3genhyuxj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3kxscicxe.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3wdsblsdf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3uxzgkhcc.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ozmqsbso.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3mvhpzlif.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3uijayuir.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3hkvmbwdc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ksbivsca.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xsbjvenj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3msfmaxon.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3htrmnall.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3alblbtup.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3wdzhdkxm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ujcbtmat.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3celtybmx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3nfhvaohc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3kcbungrl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3cgeaddyp.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3twehpplp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3subljekf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vwlyngjc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rwcivsmw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3okfejhfl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3bbnzzurh.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3lzsjqvkc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3rdglyznq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3cqbdoxhm.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3vfjazihi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ommmknaa.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3cygpdwjw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3mdqnpdnp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zxivczok.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3kxihaxtw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3scoxlhmb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3uftvwdmp.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3yvhvomtj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3qjshbvpm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3etrnsbov.html


<!-- 参考信息 -->