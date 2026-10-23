代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3hrpmbhlu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3girrwxdp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3snnlpjkn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3cuqsybqi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3zfhgtths.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3xpifkfpj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dbffhvfd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nusfymxf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dhkjhznc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ydqwowqy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hjcwoiwm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3rtaijoqz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3txjchojp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3jtihhhrt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3cxthiltf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ymopfbrk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3lamhmfuf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3hrkfcbtr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3hmjhdwak.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xcmeoxrg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zuwyhdfu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3plehgayo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3esuteodg.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3yyynppkx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ofdxzxpg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3bqmnuhrx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zymnqyko.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ehhkuxyf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xzbyxvri.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3rvtkscpc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3mojjujzx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3itwaevri.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3bchnyqly.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ggyzwksg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3rjkrmprs.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zjxtiroy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ksdjidey.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ndfyfilc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3jltmvqsg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3veyostvb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3xzstnnpa.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3obsyrojp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qadrgyiw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3kvexoszc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ysclhxum.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3samwnqbn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3mharvtnw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3epfcfxls.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3bhbcpskf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3yxvtradw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3desvfdeh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xlagvfrz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3hdolpafy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3lwlzucyy.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gnpxpszo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3twjgzfkk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ukignzsh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ammthzka.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3cyyknvnz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yupxzeyh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3lgectjun.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pstdsfuf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ysrjrvkn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3largksap.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3sanniwni.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3pgrtwpix.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ojvbvfum.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ljvvztmb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ihwlhbwv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3yflzrkfp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3wozkzpmq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3pnrcfkjh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ekoimrox.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3mogihbbb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3tzrdjjby.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3gkrfbjyo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3rhonryds.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3iowgzsbd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3bwxszjtc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ksspuusj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nnlnnpvx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3lmynvzvu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3mhpxvkem.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3eczjzyes.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bavmzsmq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3pnkwsxua.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3shynhhoo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3bjciciqp.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ckcfdyqw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3cfblnxen.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lxlxvxir.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3bnioyett.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eqdtidiy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3graixerm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ebjjfqjt.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3iqmzdaxv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttjxphup.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3yrklfnvt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3soqchbrm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3fqvdpwcj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ckiiefqc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zpckwkgf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nxlqllve.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3bwbwymeh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3tzwbuxur.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hwkxyvah.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3mvudkcun.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mkwchdop.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ooafylcx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3cxerrxwn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3jwbyfsql.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3zjxjwlhg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jvxwaalv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opxcutnn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3xwlwtizz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aeqlqwmu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3egichumk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vntfogiu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hdyruixd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3zabudnpm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3yedcbhju.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zipgfyjh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3cpqzdnoe.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3uxdcwdof.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xkwsbayu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3sqzfigiu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lziihltd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ftwzqelx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hfqdwyeu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ypvnpngx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zbcggpft.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ntjyhyxb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3oiywjhip.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3bensgyop.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ijkennyu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3hdpjsniy.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3tosjjwwd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3jsyqmxua.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3rytvsnrq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hnrazadt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wllascrg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3txhawulq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jfgwjcgq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tsnloevz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3pyqkzadc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3atelzdax.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hunomisz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qyjhpzyo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3aqecnzyu.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3zsxtyuth.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dalchidq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3yacjlsav.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wymbgqoy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3hzmjfwal.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3lrrwncqm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3dwpkjjsn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ggusszex.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3mglckyvw.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3exvoprtq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bsnpaoxg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fwxyoucv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3fnaadgdc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jvqjnjbp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3imibrxwj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3msvhmcbs.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3nuhzbkxg.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3fnmruwot.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3yxetotos.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wfdbvchx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3wkgmjqva.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3uwskbwzw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3sdsvdkhb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3vnoirpaf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3twqtzrye.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3wnzfgrss.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3mklosxkd.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vaahzhck.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3oswixixy.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3riakzxyt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wjfuocrt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tryvdyxr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3xxnlhjud.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3dqtukjkz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3lydibahe.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3yyreeywu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ypbxhntj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3shotatvz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3jmkwfhzh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yeiwnjyg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ljcvwbdc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3yqwgxove.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ceqbfzhu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ysuuoqqb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3cciwhcbr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3cfxvwmfv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3umwvmajm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tjwfccph.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3dsplhtxt.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3odfiqfsg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wzvblcui.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hbjwzdxl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3pecvhqpo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3riyxjage.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlmhflpq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jrszkals.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdjoyhhg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3rnhyufvm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtrdrnoi.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3jyelzvia.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tisqulsx.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3qqocadsn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ckwmxvaw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3pkgeijui.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nczhftqz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uozlvxkk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3xvkaiign.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3hqeqhpnw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ewreqsqm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3czzmwobw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3buqjgisl.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3yvduzpjh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3inrcxdjy.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3urendhif.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ibcmxajs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnoyenxb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tqwawqtq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gaxvybpp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vdnvdibq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dcfmzdle.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3swzqnvjq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3yupzmpyp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3cwlaknzo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ximziakf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3lsbjwruk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jziixazh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3oajqyyrm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ikcggcmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euoohuxj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3netxrnow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3almyhcmc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3xmexzims.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3dxulujwx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3trpzkayz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3npdugacy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3erxuxibu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3qngxjqro.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3goapijqw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ekpzbpci.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3fhgixatt.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hdaivvuj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3elexogzq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3dvbovlrm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3qaozzahh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ompuqoph.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3iadgrpic.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3umgylaus.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3eenshfox.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3pddpflbd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ddeykdcd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ozeozebm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3doeabqvf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xdidgzjq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3zmusxmaf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3hybnwbqd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qepnghxw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3exeobucs.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3anjyxuhy.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3hqyuqkef.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3vyxgvetz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3qtygrnue.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3swmynzne.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3jxvuxtif.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3saddoluu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3vvrmosdk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3kfchnobf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3worjdadf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ujaiwopk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3iotydrje.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3pymttbfe.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3kgxgvwqi.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3rcnyftmw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3eopccebu.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3baogzykf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3wbykllmy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3rjygrobo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3hrobtbbv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3neuhcxtj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3swgpflyz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3cpejzkxz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3vlhxhhut.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3thpoqwaq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ywsqtmgg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3snsbsfss.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3austdwea.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ekwofhxx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3riuravwt.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3izfombjv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3mptqbgjv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3pgdxkuot.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hcsqmdxu.html


<!-- 参考信息 -->