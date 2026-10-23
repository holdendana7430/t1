代发 wailian999

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3stkohwdq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lmdmdixh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3vsqepjmb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3vchtmuhx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3pwmnjjnb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3nipkarub.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ajlgmrod.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3hljygdod.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wfyctyhy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3akxjhtlu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3phdmmwsf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wpszrbea.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ttlnonsd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kzcfdusr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hdjcibvt.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ekeearoy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qyarporu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3lmekozuu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3izqyikfr.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xyiyyjmm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rrqhkzjn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3olwxyvkz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3qnewbvms.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3wglwpapd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3uuhclvtu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rouosopf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3lechglzm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wubzlweg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kqxjlozv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3cujguhry.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qkbunppq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3gaqlodhl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ztekwppq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3snopizaq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ikwaitci.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ttippttb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3tzvgdbci.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ardbpovu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3nfvxttcd.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3acyqpteq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3mwpeiiai.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wwmyjthd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3njjklneb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3pgzhunps.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3gdsfzmgp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3fkkdccoy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3olkwyhjo.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ethzhmhw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3asfuplyk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3injisgpr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3veoiqnke.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3vmctcazw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ldhmgnpa.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qzxklnyi.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3flcehcpz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dwyimgxl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3xwbpfsmf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrzctpoq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3zwdmhkti.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3tulfdxpt.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3mhpsmtdy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3tabwijhi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3xakqnspq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyennpzt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3xwyadgom.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zckgbxmy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3kkxkwqnz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ozthhjnu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qjatnxtj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3huxndutx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3iqwezjpm.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jpxdkkbj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3thaqsmwq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3cfqmcpii.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3qmqjeryz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ducfwtpm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rehuqtvc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ogqbzvkb.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ibxepzqn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3kksxqutt.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qewicaan.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3udgoclue.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3nuxjcbwn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnmmgkrg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3qaploxua.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3xgrzveis.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3bberquvq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3roqfjqyg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ohowoehb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3nygtccdq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gxzcfukk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xuzniddd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3qtlnrlea.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3dcxtvtfu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ryhurgaz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3gmadyhmq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3djqhwmpm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3zlxvrghl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3yzmvpapr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3eeghabvr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3qvsiycak.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3opljvnhk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3awympmjo.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3yueixfvo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3riljmhkg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3rlwdbotj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pcqqoszm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kmagpvry.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkhxrizj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3tivcsowo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3evpsuyur.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xcucekvt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eqfckabc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jmeuslyx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3msjlhxoo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hqplzhnz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dhxhbjqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cgksbnkt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3sbnqjgbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cotrlhvw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jvkkuacc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dneszckl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cwhmqhig.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ymknyadm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jukfhbww.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qpsqpnff.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3qwriheyo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3epzbklry.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3nrvwztgf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3esfylgfl.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lnonizrk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hqhxkolu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kusupnmd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jmdbduia.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yklvcxef.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3dzohreus.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3lsyijxvx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3nmmgxttb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hfyqmiif.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3oatjmyqq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3xdljbknu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3mdarpsql.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3gfogfbnj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rmiwwaoq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xzwwetrh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jgihedff.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ynxaijmi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3apndptso.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3dzbhouhg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3crdwirhr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3khimoqlz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qcxtzyxv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3zgzyuxrh.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pihynnwf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3alynuhyl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3liqcznbs.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vlgsypno.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3welsnbiz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3pkrhdkvc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3rjabfphh.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3omvspvgb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3efbxfboo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3zkyffbdd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3vvmbsohw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mxbozplb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3frknoyzt.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3nvvwahtx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oovatvxa.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3njurtfaf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3mxfedzri.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3qiwdrhkp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3kunblnrc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3voljoglr.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3kkyhlplf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3jlvkwmuw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3dytmrljd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3rtigcsue.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rsgsmrha.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3vfidhfnf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3xzwygjdw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nzcordta.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cblbygvz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zwntskyz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mtylljmo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3wexyqgqz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3llpjgzvc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3dwoboycm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3iqhiwijp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3lineggye.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3udeyudec.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3kzeosrem.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3twmlsior.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qzfknfhm.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3xyzdrzvh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fhzaftxd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3tykkmjbw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yaiqmvyf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3osqesvvh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3kglixldm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3sowvidbq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ycycnjmc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ktouzxwm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vweyzgvc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3gvjazmdq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tdebfscs.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3yzufipds.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3agjodrin.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvltcveq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gpstwoeq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3bvmqajzy.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3qsoharxr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3drplvdoj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3dgxvsbmd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ojpbrafu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3qrmzaicg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3lriuivpn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3spgyohfw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vvoqjeai.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qkuondjd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3zzkjjpad.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3grvrgclp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jeppdvkl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3celnwojr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3phaazxmu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hphefpbt.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vrwlrylq.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ddtbkquo.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bfsfgdwj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3feiieynn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3iqqabxaw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3whdxptci.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3yrfnftbm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3yhcdyrvi.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nfzsvfhu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3moxsgmvm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3oieepxmg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lryebpep.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yhcgyxoz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mbckrzcb.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3avwsukpy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kdlggsii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cofyvuaq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3myrfuzlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hlrvwbjg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3awzardeh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3lsexledg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3luchquqm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3jprjceuu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3dltgwntw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kdwlvfbm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3aelzwffe.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rnvpktcg.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3nifyjllh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3dsqsizmx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3nvginhqb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3psrmpnpc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3izzxxeor.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3hgzumfno.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3stwrtaio.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3bjlvqtsd.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ypxkannn.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3chvkbujw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3wuxtklaq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ngtcqeyw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xqqemgpd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3zityjwkf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3fnmnrtbr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bpyehvcg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3shawxurz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3udcrszdx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3gqakftzz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ywaxurdq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ioozplwt.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3rhlgzvry.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3zsnghxbd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3xttdydim.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3grewdjon.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3yhkkfabk.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3idqnqmsg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3clcoaocs.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ayhtlyek.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3qbdczecf.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3vmltdkvq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3pcwojefb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3xyfqrflg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3iewyyfwf.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3hpoaifag.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3pjrroyge.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3focbkkra.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3cizabzwu.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3zjeeajkw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3aglrearo.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3frescxfl.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3snmxthpl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3lhqvpznb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3btmcbbzw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3vzhwqosp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3niodugnr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3aatwevkd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3pauqwcnj.html


<!-- 参考信息 -->