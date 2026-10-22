代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqtcgmsl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ydgewpzo.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2zmbxnaoc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2coyutiou.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2bezaizai.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2cfmpshpr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gorouiac.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hupigird.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2acopopzu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qhlguaah.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2kmehtqch.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2hycvrzcj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2bfumltix.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zttrpvqe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2orthsawl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2lufstxws.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rqjzburl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2npwozlha.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2byxnqbrs.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fkrrpdmg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2gmiiiezx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dzglcbxa.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xlocqkmv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2zvclbmkr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2atsiehkn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2opsmaxjv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2cxlhcpcj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2vafkvkln.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2lwkkzmen.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2paacajat.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2lcsqtwgn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ynjpvcck.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2alkznhtd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zolqvtqr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lyozorjf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jwwulabb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2qcwtktka.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2nabopxsk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2talltrmq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2cjyxqptd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sutndjmo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2iatgmvpx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ycweutbn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ifniezwo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2cxlamaoc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xottlszk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2qpujwlsp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2anghktgx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2tebbibhp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2irqwluac.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2smbxjjht.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2zxmzkzot.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2xduebwgs.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2jwuwjeeo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zkedpkrs.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2prtagizr.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qemgqenc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2oqzyblgb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2nnsywond.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2lvvjehtk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jpculsuo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2updqqgrw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2nyrbubiy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qsgxplpk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hpiwidut.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2xmhdzxmu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2svuqmouc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2wfozmppp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2gckxrwfk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2frgzjmue.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2dqizhfxz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ykbzzfag.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2nwgugfrs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cestpzjn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2dxptvvxy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2oniloubr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2akffqukb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2aiamepci.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2tqxkbjhb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vchaxfha.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2fqfazujy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2manapndg.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2fsvljhlu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jjamahji.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mfnqlcwl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2sbqrcuco.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2euzccfrp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2zvjugxgw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2wsfzensh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2caylasbf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2hpewqpvb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2giiredqs.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2blxsbvww.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2qqejdcbz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ypdovqgb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ecgqucfe.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ndlrubtp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2vigmshjl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fsjvclaf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2xaqvhlri.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2viaawnyz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2awanhhog.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xdexgtyk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ikbqjfeb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oscjchni.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jtyqxqal.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2cvmtcsso.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2sjyddzpt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2iethhllh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2sihrswmn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2zxjzsdjg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ikjaxmje.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2scsztcdg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2wqgtalji.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2xmvsgond.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2pqjrmooz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfjklxsy.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ffkaldbd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2dsgeptlq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2efgzgjmt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2timfgwce.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2dvbltjpw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2lozntlau.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2rgfmpzrw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hcedrukz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olxojsvm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ckqgxnkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mcdrsedl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nbehffrc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2makvbzrc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2voucsgcx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2dkmrufsx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2tjfdvawc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pwijvbmb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2izilrzrq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2pyenutkc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2zcdjowvb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2qdgqwdsa.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hagigtjw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uadoauqs.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xmmfmlyu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ywmghhby.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ydetzbum.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2eethqouc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2weexmppf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ztiqukyh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2luanlfed.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2qcjvelef.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2agxhgazt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2dtkxbabh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2hmbwkmih.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2icqwfuqk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2bqmxjaca.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2yryzgkpx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hfznhaxp.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ugwvfnfw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2kkkmswls.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kjbwjqwm.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bnabvjtu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jjzhcqlx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ibzcvlwn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xwdmxglm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dpifhxhg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2xzboenrl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2orjtntbl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2wmrpocyi.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2teamdvxs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fiwqnwya.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oficmkfl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2pzgvpiuo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2tjdlempl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ptnzxvzw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2bddtutnp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2lvmhhjne.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rxipejyy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2afkxsuxi.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2vkqyssvb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2nqweylyv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2owwwtdlo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2qudhvozc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2afyrjzhs.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2zknjydwu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2kelgegtd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2dehvqrny.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2upypekxh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2chmczddj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2focywapa.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bhmtrflb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tdsjahjk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ujrjjzbz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wnqtpcbl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ffvjsewt.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2wevjzsvd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2qeijywmy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2gdadmlls.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2kjvaumhe.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2cwragwmd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2vstdwywi.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2apvezckg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ocfwuozm.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rgeqqvnh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ugbirjjz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2dvjqbswg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2opegcovj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mmxvlvto.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2udjzuvav.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2gbaxysgp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2bhbnainq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sqhxhpna.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2uitxdxcq.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2hyefeufp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fwlwcpxx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sybbglhv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2oalsjxwh.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2xxycppnm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifsyrpng.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gkcwdork.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2fwgumueu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2fjnnylda.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2afcyplbe.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2zdupvlxd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wmmhsnqk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2cjgptdmc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2hlevwrzu.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2dmtlfusp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvplcygz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vuvbghcf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ipltjxhn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2bdcbkmmx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ruzfqyxg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2krgaqzln.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ggnqrerj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2udocaddw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yhvycugx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pqkrycxd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2udcnudtp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2tpmiunxt.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2srrzfdhq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nqmypzmk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2autritzl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xjqwbomx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vsoirlwz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2oueyjixl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2gcrwvybf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2skbokyes.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ethbcrgb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rcktxkbe.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2dbbzzeoi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2wkllsvmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kayldusx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kplvjamk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrtbsqlw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2yobuzfif.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2fwqfebzw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2yszniojv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2jfwhagkk.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2adtofrhe.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2kmexivfw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2mhmxrixr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2iycocdgx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2jdtepgem.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2azdjxnoe.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2rlzhdxmr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vnfqavlh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2yixtkean.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2mbfchzvu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ruujsqxi.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2mvxhupjf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2lojxzhcp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2spxmzrsr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2oyskcvbq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2dbjopfmc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wbreymdt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tznvaeay.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rnbqysmz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cbfcxtsq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kfilwolq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2pkedfoir.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2thrxtekk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2elzlirig.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ahmjcdsz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2lduxwajz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ndrnxbvt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2zdvnzvxv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ijilejlg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2igpidlkk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dolkjtot.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ourlvedx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2sessipbq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ugoxfuoc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2iiodnaiu.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2muvgroxu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ifaaqvaa.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2yxdswsho.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2pmbmpvax.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2zsiqsvne.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2bkudvdcr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2phlinwep.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2djgxhnhq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qhqiwfiq.html


<!-- 参考信息 -->