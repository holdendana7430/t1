代发 wailian999

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jjnetztj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3rvtjjbck.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3bydahngz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pxoralfc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wbckjmqz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yfjnmvji.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3koxebyip.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3fhlwhfxt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3vyeikppy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3nmtkulgi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3xzzczzfs.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3stmtmlmg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3yprhhifk.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3rtkuovyn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pejioais.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hormcgty.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3yoyrsjcz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3urnnhlil.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3saceehrw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3thapptin.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nkdjpmge.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3botxvxpl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3mtnfakqd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jzwgirnn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3aqevkide.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3jzrnpnhc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wyvbrysn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3khcstwjo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pdgjxfao.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jxtwebgu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3zpuhihiy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xhsodvwk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3pakttxbm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3kzqyvvrn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ilzzwvjc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3zcwvhhmb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bhoivjpn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3uonuaelf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3kjqgriwc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xleakjro.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3glgbrgfy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3eijogdpd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3chncqdxu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3gyrgwlxp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3sfecxdcl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lzqwkebq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3cufkyrha.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ihenhqsw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3kszlvgxe.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ohycsitw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hyqqbfek.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3kklgieet.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hljrdvdm.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3btfutvrn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3kgndbxve.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3iwjcjrwr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cgrhwjna.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vdfawzeb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3gthooqwf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dvntjvcn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3unfhpxei.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3mmxatjcp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3pvogtdqf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3euwjppgf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3vuobuqfw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qbfxmrub.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3iyceaame.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdmnwhrq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vtchchbf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ecmosghw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3bpwxshsd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lhpjtnnu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3voclmpke.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ntklmfjc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3oykxtats.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rvteknkd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3jmxvgsor.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3szaoxaxd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3angjvbff.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ahunjmqf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zdojoexg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3hutrpcbo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3gtrrvmsc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3bwlyxjjf.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3heapmqjd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fuolzmtr.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ewtwnyzo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3getajgdk.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hyrpkxwf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3nasvfpem.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3zplhtyji.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3aazfrkwl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sjofjycr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvhegshx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3azdwgofq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3jgzrlofj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3vzewqwmh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3neeyontq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mqwkyulw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3vyjlrqus.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tmwrbgmx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3iqzvuuml.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3udawotkk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bdjpxvdv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbjoqpmd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3rxptxgbh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3hjwjdgxt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3eqlvhgqh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jqujzivp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3kqxfizfd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mrbcbqrl.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3djmocwca.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3pgesqysr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3bmzbgktm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3dzkuviav.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3mkbvoizh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iolklypu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3pbuydfkk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3nodyzjmw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ydehhhdp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3idlacvdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nuygiteo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3dvtqlhas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwsnfqje.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wlsbdtum.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3woijvcye.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3khqxegrk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hyhcjytj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3rvdtbmpw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3msxkdwnw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bflpgexf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3smjfdrik.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rqdgasfu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3gdvodcqo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3eitpfspu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dpgwhtqc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3phwbruxd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3idbeatjd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3otudiyzn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lhpoxnyo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3shjlubkm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3zdjycbsj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ewwzoysa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3gnwgrafm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ljoetkxs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3xrqknpnl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3bjwhlllt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dcjkgriq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3apipxfsi.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yskqkufx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3uhishpux.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cwcyrnur.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3trztmlty.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3voabsrva.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jxulvrhy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zhbhqumt.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3pjwpftng.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3suoapiqu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wfqfhhnt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3vtwypugm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3uperuxdb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3uinskkhj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3vzhzrnnk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ilkserbn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rqndhwfc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3xmusbhth.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ztvncbsv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zebrrkey.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3zfpckbhk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tlskkgux.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xswxfkyg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3axoggdjo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3avxrfrdv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3kcypiaqt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3rabzoxcy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3debknxjn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ixgpxtfx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3cflyrkdw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jrzshhuq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3mppecubq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3omtgcqgn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3kuoqbcge.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3vixauiyu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vzuhfkyl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3czlgrplz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mlbpgohb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3lqnyujmo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ualmfrfv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3aekdfhac.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3edatswva.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hrdpnijc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ojlssceg.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3wsepwavm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3utvwqbqb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3etqcffin.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3apgskcll.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3obhmgziu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3mvazekdk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tkxbebyf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ughsjmuk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3igcuhuzx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3jrwdwflh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3kqwejazn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3sijbccyp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ufcgvtov.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3icxvcejv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3fotcdlid.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qorihdia.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gexbtbid.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ftkthmqz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lixmcjxt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3vzaipqzi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3mirhpbnd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygvorlvo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3nhnfurle.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3thnueyqx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3woxhenxj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3nnchpxdq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3yxvnkfyx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3zmjtoigj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qvqfxuca.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hkabuuti.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bjfstpew.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3mxckrnnv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3lhjyrxca.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3scpuahut.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hbfentke.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jwcomaoy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uvtjfwjx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fsavwuhb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3pslodfiy.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bweoeaar.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tsspnlnq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gsxwmixv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ukpqjklj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3rdjiqjjq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wzcrrrcd.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kwtrxjch.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jhspqqsh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3audcxdfh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3gvhnypwe.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3jhjfdkzg.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ycnkoeef.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3rmctkpwh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3vvanhqgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfswyaac.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jeoovrxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppeeejni.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ohkvenrp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3hbgksxoj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3awrkkyer.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jclkyocq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3quodvbti.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3gajjwvwk.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3kyyihakf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3esvphljn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ylijdwzm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sebqnvlq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3pqwasbca.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3pvefwcmf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3mkvfeujo.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3qmzibyfq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3coqlcfag.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3rfnlwecz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3qhxaucvt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3rltpgybz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3rwjurxgn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3wcuhufny.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3bzhzhfuu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ldwfhwpq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qldxdeqh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3oetoukpk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3kinqivvc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ivguhhwj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3tgragskw.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rlqbblli.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3eclkxwvd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3fgrprgfg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ttzmafmx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3mbckcmun.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3rrjejswq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3rhptxexp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3thselilc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gsvcaqjx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3vuvjsefv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3nohrofph.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3urnlaldk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3qhsoulxu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3cnpcwrqp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3rakqcemg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3myfozahy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3uzlhjtwz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3rsuopaku.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3kajyayis.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ponfzsrj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eqpxieir.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3zwgidouy.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3txhhpyan.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3cdytjqie.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3siygencc.html


<!-- 参考信息 -->