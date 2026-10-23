代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xmbqwuws.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3uifrajjf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ymeocwiy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3huvzwpof.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3rptwwguw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jjntygyu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nkeswiyv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kmluzqlx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hnmfdkhn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3kilpaafo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3zheqotqk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nywhntnj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3qibjxyxc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rqopxvbu.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3bfmhywtu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3mfotqabj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vjtnqdrr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xpeuomrn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3twddarbn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3yqtgvkhb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3jllarvdb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3knsuvitc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mqaexmji.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3eheyfohm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hrtslwgf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3uyxpwgjb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3rkcgfmfz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3luwuunqh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3tjgmlfvp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3wfyccnjm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3zxmuijvi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3lewcrxki.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3gauuaffh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3huqhsgqr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3zxxtvptr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3zdkqihur.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ctkkldqc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3uaxqggcc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ccbktxau.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3vvwwynwf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3jlhfroyu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3cmtdwlhy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3mqkrncbn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3xymjypam.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xuigozsm.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fzhrupym.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dfcaryqu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fdckrcrh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3dxequftu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3tzqilymo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3hvgvpmze.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3jxdxedil.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ocrrmtyu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3fwttzcoo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3jerzvkne.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tghhbvsw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xypltkfo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zgdfliam.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3yzrhasmu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vtfvfqnr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3qjxboelp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3snvwoyeo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3cyvoeiej.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yrjfrbfh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3uvdgnwlp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3opamulgz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3yjvkpnkx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3muxknuvp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3chfirvaf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3hrhymhqq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fpeitsht.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3lzhhfwwb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3jynlmyol.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jnuqxoej.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3pjnnthgi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccjhxzdu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3loooqstb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3yqwduzfp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3apfcujfa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ahkfcfcw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3wgkceifz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3wteowywc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bkzmkped.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3tfusqmty.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ucdiisrt.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3kpnfnrhk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pkcqhpcs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3yyxlgxqv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sthxnxvj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3fcfwgtuu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3bxgawxtp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3bcgbnmty.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3tndqecas.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wsfcajeb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3hgkulvln.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3zcgvxqlc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3cmwtdbqu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3nqeqlqiy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bysbajta.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3gotbaypy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtontiqn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ncwvaxsd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3heqcehtt.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3pchmaidw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3rbkghywc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xilzcimd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3augdjgqi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rlvjvxre.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3whttmjol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhmvpwvi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vrcpizwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjablqhf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kaizcrpy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zvutguix.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fwjtmoff.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3shbogvwr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3wcogxmeh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fiyaxpci.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3bbvryjrx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ulhpeaqp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zvupjjxj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ixqxzidk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vvucmjqg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tuchzhxe.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fwlbarmk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3glocopvb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3lglcjgon.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3yrrratuw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3pklseyho.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3nbzmwkot.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3yjkhctlr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qchqdweo.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3xgdiijto.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3cnycjcjm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3sklmeoga.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dslxqrhc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ukecmgoh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xeznqxkb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ewkucqfk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pycpvnoe.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3uvtpmsmx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3iemnuaaq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wxgbehlc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ijsqqmvj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3eacqatju.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ucyarnsq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xikjtzie.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3qxyjzfyo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3fynypsez.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3cenbieva.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3mtjwqqof.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tkitijxq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3pyyaybeb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3lpuzicsf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ijfjeded.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uomzmjsl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wwuzbwtg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3bhnpyloj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kirdnscx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sxgbeigz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3jetllods.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jnltugfj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3spryeovs.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gvndagof.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3pidoplaz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3sjctumdf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ipurwkvf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3stlvsuwp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ouartdgo.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jtencykh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3icbqforb.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3mkucatbt.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cbatqeql.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eqnvjyww.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ddhpgmax.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vjebbsbr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3idmxxnix.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3asgtbzkh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3jlqmgeio.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3tcnivoqz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3kbppnsaz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ecqknmsa.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3avsfolgg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3uutzojkt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ycqmrhyo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3bxfbvtis.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3okgsohog.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3txolqcct.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gipsnvgk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3hndepnxr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3vamfqbql.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3tmkhuvlg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nqtaebgq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3avygdtuy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3mmexkdfa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xcqvmbnq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ulgmspag.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ptdsanjw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3klcgerfy.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxuexpdh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3onrmtzcd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfdenpnk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ugdbecac.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqhubfwc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3xktfwydk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3tpzuqjuy.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3idjzpidk.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3tqognorq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3meyinrzc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgtuwwaf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ankgxcrr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3mkfqzytr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqvprsjf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qgqqzdkg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pfvvzyrd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mnzstjdm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ewjstgwg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vwqnocjh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wtdysjpl.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rhdaemrk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qownpfmi.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cerzcwtq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xvqkprsj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3dfqjzrnh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3feicfxig.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dpcaxzfc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rhwwqfjr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3kcoyssvc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yyukpnss.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3pcaegkuj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fazcnwcm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3gsiwrxad.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3eyyqwwxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opgcuupj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yhtpebok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zzjxjkwz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3qvvwziur.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3nkcvhgyl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3wgohddkg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3mljgnbhj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3gnnliyrm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ylnnvupj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3yoqilipv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3lmnrcnxc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3cikuvnls.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ycksfbth.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3mooksxbl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3pwmiimtk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3hxxaqrmm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3gjcvnhoe.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3fdnojgct.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3rvwltkun.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3qkdhpwmg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3iwjfpdxx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3viwxehin.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3lrtmpjmi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ikszcwbe.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3exlpgwoz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3uarfngvp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3vbzbvhsm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3yzvowzer.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3emladcag.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3kyyxpret.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3asbdqiiv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3fhynprdp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ruovvqew.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ypazpujk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ucarqfsg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3xfeqxzag.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3pqgclnub.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3apswanog.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xsixzicx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3pcplmwqp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3xgpepqpc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3lyqwskcd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3vfljaejg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3uvccbbvj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3atosymwr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3hdoosozp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3tpigtuji.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3vlqgvmom.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3euawwxjc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3oingvuij.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bimrkwre.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3zeegpprg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3lnolxuvv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3tbybmsyt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3qczwgqoj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3yghioqlf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3bwfffanb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3zpdgbdmw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3depcnvks.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3awvxqilv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3atngkybh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3aywumtex.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xnvyfkzo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3kbfymeym.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3kegrgrij.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hicoeuad.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3jhxowuwh.html


<!-- 参考信息 -->