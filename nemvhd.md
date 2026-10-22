代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2vfkfhdst.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2saggtjjk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2yzqftdpz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2dxhbkzdy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2tlybfseq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2uhgyicjp.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qmpgzxro.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rhqzysyi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2azcpwszn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ptbdgnmt.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rjebqjiy.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2cqzxjixv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nwhsewwy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2zjgtfedd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2hiwtiuog.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2egclgdid.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ghaexlry.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ahrdbpxp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2azonsfpt.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2zygjxlfi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2stbupoph.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pmoywawj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2nhlknaqv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lbywrebf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2mtjhksji.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2mczqxmvx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gwzmjppj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2dedqqkej.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cbdpkrjb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2llqowuzl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2bixavyjj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vgynbnrm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2wmrnzpge.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2zittangk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tkzbbpyw.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2qreczcaa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2vovomgru.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zaqknpkm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2riwmthkg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ivtzfhcu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2hunpotpr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2mgjbbcxv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pvtlmjlb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2cxhinznn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2agtfslkq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2xjwkjazv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2isruvcaw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2isdrttah.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rcytyqdn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zgejxfzr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2mbnoazdr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pgobjbki.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2gesarpxr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqnleaiv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2kbamawmu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2crvrexqt.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2eexhgzxz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2dyqhlzfx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2lghsycdn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljxumwaj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2rgqahkov.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ulkpmtcz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2qrxsjgwq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mugmbskh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ciuxnsxb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ajpfvwaw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tzfnjakw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mjetyzol.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2thgvqnti.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vubwyjzp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2kqspethy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2gwmeaiqv.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2lgvwachj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2gneljilg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2bodvupwv.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2jqgunkqd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2bqavmktz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2glphvoou.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2zrvwmlzd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltoghrum.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2sjilimel.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2emhzgjrz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2opjeqmvr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsptjsvo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fkylbqkt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2syvdjvuk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2besxagfh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vihldssk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wwbclxtj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hkihiycr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2oygundyu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2pastgmnp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mwxmuwsd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2obcjazml.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2rjwxfzyd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hwknoxet.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qtdfkpxi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2esbihbjo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2uljtdgbb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2bnsntfic.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tppyoebn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cjwjptjf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2rboeklyf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2wgwwfnax.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2xahtarbl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wszbeneb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2faliwvml.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lselsthx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ynacckgd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2dvwribws.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2jjabbwgb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zivksyup.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2juqkaddo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yinunfvr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jepkhqcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezzvrebl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fixvskyo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2oibhuurl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2sfgqctce.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2pcwyfhkd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2utrdndie.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2arndpbyd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2budoprhj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ikkuaufb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dgtxstlk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2vtnxaouc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2codzdeeh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fzusxbjm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2chejxqsb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qwkzhduz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2wnolvcoz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ctxsryfu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2dzuytakr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2mgbxcwya.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2mcrcyjbp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2voonzxhv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2kiofoshl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2fesuimdl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2avbngten.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nzuxybxu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2dtqktenc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yrxtvtvh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2rnubrypn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qryofqmm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2peaxrouc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2dnnddgnp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qddqsosw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qlrxqcgu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2simzizsj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2izrrdziq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ihvsgwfy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2gucwlvao.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2rkyezwja.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2yevgbevn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2wonflova.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2izwsksck.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fxgbtazj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2uunjcszu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2vdfkstyy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2dyulcpjt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2tnxtblsi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2xszmdlvt.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ueshqtqu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fauagxac.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2sdhtxzng.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2fhioqfmo.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2aoiudnjf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2xyfzhzdk.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qqmiprzp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ppnwvmaw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wtfziqcd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2tjpgmbjg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2jtukmqnb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kptanbdn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ojwffoya.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hxdijadd.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cpihwvhc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ggrkdyna.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2zhqgcvgr.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2adjctvvk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2gqfratud.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2prhsonhy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2jexncsjx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2limsnbku.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2blffbyih.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rddvnsjq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hdvbopeh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2awwgptev.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wqrxkggm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2erejbvxj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mmeqloqq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2cvtjpshu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jrbtwuxy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2axvdylxb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2yjllhykd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2cwjbvlkk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xcnhaqxq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nsyaauoz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qborbhvh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fpiduxvx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kahmqfin.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2zstrjrlu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ebhncnzj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ogvscmjc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pkzetkep.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2awqefbpz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2jwrretle.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2fgeaagnm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2hiuytcnv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ewtngfee.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2twdfigxr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2kzxfxqqi.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2cofsuhgf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmpbhskf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kgnuebxh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2elrxmurf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kykwkzpn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lillwcas.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2szbficzh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zbyteton.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cgzpjsua.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vsjdksxe.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yvxuepok.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hhgsfrqq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ihjpzbpk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2punmbrzu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2uondimjs.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2twkuelli.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2etzreunt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bmpdvyit.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2msxceeiu.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ovzqphby.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2lnrgifvc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2rmmcwhce.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2iyggxjxi.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2wjnyzbhg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2yusqmtzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tjzmbpbb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2sazkoxhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2myyvpnbo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2nymfpbps.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ellvmwjv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2loyxdgan.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ehpmceow.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qagmhzkc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hkedeuls.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2kjbopgmf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2likyebpm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2avtbrbkb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vxrkrsvh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2xbieogud.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2szsfqjnl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rrnolfuj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2caavfcar.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2mutzsnck.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2zazcqdcr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2jezbccsu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2opceaeeq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2dmklvoyk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jrnwiauj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2mdwrqncm.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wflwhioy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2tvumaunn.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2chbitfll.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2slppzyke.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2rkewjoiw.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2rupmxczq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2faihjisb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2gttqgvlc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2drzzokiw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2yyegfgfr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2nmhgxvzp.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2rxdnusdy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2mlhcogvy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dwphkzgl.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xjnflbrf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2jqzgkpsj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2qcbwvfzp.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2yerwwygl.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2kxafhtuw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2glevlqpa.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xmhyqcgk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2fosgtlcc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2nvoohsha.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vhkhtjeb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2megjstpc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2svajxbvz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2sgbsbozs.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2jwafvajd.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2bchjefuf.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2hjnokvtj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2jgqnmnth.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2eyybwvyc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2osqsnfoh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2podwgejk.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2nzkospxp.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2yhucnljp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2yrxxwmwd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2vloweczj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2holkmkne.html


<!-- 参考信息 -->