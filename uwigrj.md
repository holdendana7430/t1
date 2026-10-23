代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3kzebtgns.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3zzdzusmw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3dazzhuoj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3nydnekst.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ozqwxxar.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ibnvnnpb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jjavccmy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bsqrwwnl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hpnzahsb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3psuukpen.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bnvedebr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3bmhrynym.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nctxusnj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3adbqcflg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3gnihibwl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uqfvnpuw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3cxjkxghd.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3zlctulzg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3gtasujmq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3omsucvxf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lgunjrfw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3luftgjdc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3fthvoclp.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hpmpmivb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3tpdrhzep.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3fwwxtvnq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bodmdniy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3vbmfntth.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vzarzxtr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3savsjpqz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3faovauqt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3pidrbuqg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3knoiepfs.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3fazvjlar.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ougjelso.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3vwoajtio.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3bzyipeiz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3avgenvug.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3lyuncyim.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ykkabrpq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3cgmaitkn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3xzgntkfh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dzaminru.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3tvipfrcf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3nfkyvyrx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3rbjxihas.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ielrglin.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ztkfcrxe.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bgplvmmx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yhrvhlug.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3edyntkik.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gjtefens.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dtuoxovw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnhblqyd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3gchzknho.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3becmydqf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vfmyppbf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3uwqwznej.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3zzokcpdk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xmrhmivs.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3gwuwrfyw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ielejfxb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3judckgkr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3swstzvev.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3orldpaeu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ulfwrjgk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3pmodspjt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pzecmbir.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xzcneozt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3rprmcksk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3xfbtfori.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3efdvnsze.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3gqfvuomb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3kfbcagme.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3zhuslras.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3tvdhdqwi.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ermwilur.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3zhcrzcvl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3kvoigtve.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3adpbebvb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ndvffnst.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3wydezqbh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3hqqdtpix.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3vmlkeslg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ygfnrezk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ldkotlzo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3btjnkogi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ddcbkzxk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3mehlkstd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wuooujuc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3nveojzsz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wbctwjro.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3stalnikr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3exbdfdyb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3dbpanhzr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3sslugfmz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3kzvuhzlh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3weyfmlzd.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3nwhtcidb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ihlzyecr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3cepiqicd.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3rtjbgenz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3gnsaaumy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3rmbvwklg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3jpnmdxdj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3cjieolsx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3pmhzkzms.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lwbxrwbi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3pvdolrsl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3nhgsdxhi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ztmgfhpl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mevohyjk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yimtblio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czjaalgz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zfbcmfqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crplfvun.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3efqosevq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pwjpmreq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3xbjijdzd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3fkrtimmm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3fqmzzsgp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ncpetxsg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bjzwidct.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3tcpwovpt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3rcuqgixn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3oubaqyuc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3yynsbbhk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dgzmicxa.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qqsuoxor.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kgbyxnql.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3raaaeazf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3omgdroyn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3lkbcdsac.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3tgbluwpj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ggpmsdxd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ujpxhorz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3hnqynode.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3qudfbelx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3sduvnzck.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pkeettsf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jwwcjiwq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3lbofifzn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3axbflehc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qkahqjhe.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3xnxbmorc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3itdhtflr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qqhjkdkk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3aicsjois.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3bvuvtxhu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hvzkrwon.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cxxgrwqe.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3kdtbwilz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ufdeiujt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3joeaqwlo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3wwwaespw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3gzuvoyoy.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ixycedlj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3undlpgca.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3felamysr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gklgyupv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3bjykgbsl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3knuytuwq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mbqzabzj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kvbljroc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3xtcpxfvo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ymozkehz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ghzmahja.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3kujqjoar.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3tmledbzl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3vmonsfqs.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vcqemglc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3pgjwwgtw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rocumibq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3sgmlxhft.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3pvmuexmz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3uxquwtqq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xmaxkmly.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kecpwggn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3zfqvxtjp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3vuhuqigi.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hzifppkv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3xfbncjwv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qzbtrjdm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3mncgpbov.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3yevhntxt.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wbjjdbhj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bdgrslge.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3edstfxwe.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vqvjxozm.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3hgegazen.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jshsqgag.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3alsrsqso.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qzhopebm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yphyqmqq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3rgtsjutq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3rnbejdip.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rrdxiyfz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3nrgpcxax.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wbserkrz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3nabiesnh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nhgsunnc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3yqxowmbr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3orhweuqk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3czczarqc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vjntpubh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3flqfzttb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3qgydbrgq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3zxjmuweh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3trnophgj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3fuvsdtbw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3peyandmx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3iylfmbln.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nfnuseaw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tjonenrv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3giksyzew.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3bxoojzkc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3suyfeeom.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lbhygpnj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qfvvwjhu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kofxapsn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3olurtpzo.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pfbkvslk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3uwwtzpas.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lguyrqqu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wydbvkne.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xhksjnbs.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3izptcial.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3cpmfgptl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qetowaqs.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3smzsuszm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3mimheipn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3wvjuyfqq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3tqapvhyt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hhpnfvkx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qhwnmzuf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3mwqgissq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3cfyafezc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khfpxzzl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ynqemztm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gebotmqp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3mrcvnftd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3whlfhvsa.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3gycxkyqp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3pkzzrkqa.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hcwsrszd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3jcsndggf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3nhlpapew.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3idaflcda.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3bekfuplt.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3evzyqpte.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3quvccvvo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3zpptbdlk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ovszgltt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3wziwmrkh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3hcgheafq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3qahrkasp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3mmrdkdxo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3bnoneetj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3sumpqcpu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3odknqzbm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3rmpcklnb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ccohzhgy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ustsryqx.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3adtetimo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hovrrfmx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3mdgsyisp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3tjjizfml.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3qjusreoe.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3posxafim.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3gmeuhezj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3yvpzpyty.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3rhefzaxj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3whxexxvc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qpbcplnu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3orptuxbg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ktyhgnzb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ccreuysz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3bajdnqwg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3mkgucbwm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3fbbeabfy.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3uhgafhsk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qfdguhak.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3qlpsmlko.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3axkrtpwd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3zldpiots.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3anewmhid.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3nxzemjkj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3obrqhdwm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3gsflceja.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3arlsdyah.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3hsyuygnn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3kpqpexlw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3btjbvlkb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ejksitfk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3uopihqvl.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3zskanbqt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3pmhgdhww.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3sbcigwzp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ygxhmypv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ipdngrpi.html


<!-- 参考信息 -->