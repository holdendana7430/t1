代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3jjweubsc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3xhnvtkht.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3toflymgl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3nsoxabjy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3jdjswnnl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wwnvctpf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3shxyfivf.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lsupdvon.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3rmlhcqkt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jmdgpxod.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fhldlzjl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vymurajr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vrobyyir.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3cribdydo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3jryojpkx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3eicqnigr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3spigloqj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3nuicpmed.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jgcotzld.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3vsifrsbu.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3uaemhmhp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ibdncpuu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3dzeqonjq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vkkntfts.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3fgpojdvb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3dyvikxpx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fyoimbnq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3drjckpxi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ipmhdsjl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3zxylvadl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3sysaejoz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vbfkkkku.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3igilaglc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3nxdumoho.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mdrtgjzf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ccwfvfhr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3avgkqods.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ucfjbhlo.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ghkqzhmx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3hkptzcei.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vtcltexw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3flomtxwv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eensgaug.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3fkiicyby.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gbtiutai.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3gdqeubvg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3hcvkbmru.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3xbvmiuom.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wlbngffz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hmjnyonj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ppswsniy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bknnvlei.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3oxkdupmp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbpcvwom.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jvvxnntb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3jviswwro.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3xibbtmim.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3rwxsjfjs.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3uyphtplc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3echlawbv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3hxmxcgrh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gxlmrwmr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3zxkxsebi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sxfckztb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3czdxdgyx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mdjfvzwv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3eoqvkxus.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zssmkhmf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3obcmabpp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ktjlppkv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ilwhyyrp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uljemfly.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3hxxzqqbc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3fzpnokpy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ztxerxmf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3szzprkfl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3opxuzsjn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3vhibtbtv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3qyqynahk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehoucaly.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3foumhxen.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3wrqwsdpt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3yicavgjg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftpyitrs.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3nudhpxfd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhwwbfsy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qhbgchak.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3apdrtkdo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3nuczqprz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3oamjlezn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3flvlbpte.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3xtewnkqa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wgdtbnoj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3bnlcphau.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3cpuuyagh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3xqnsesmi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3kluxsegw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3yfcfmpao.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3lrqvjayi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3psvqcmsg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3chqddmyu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xecymlpo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3elhbizgq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ergxhxrj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsflkxjg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qrmzbgoc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ycfvcddv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3quzzglcd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hkfsnbxo.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3pwkawkmk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3rhqixxnq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qooqging.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3kezaorrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tiqxruls.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3hywdqqqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsnhmqej.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cflgigms.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vnngkmdo.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3oysjnput.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3rycohets.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3bnvulaot.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rfpsnmcf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3epjnyqnr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3gcrtnbih.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wbjozhvg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3bxpbqtqu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3eoidwinf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3erzdkrny.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3abbmlkhj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cmhnvfuv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jfejnpzv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ebluezqp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mhpyolrj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3kjlbolww.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3nwpuhmgw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3csuuqvye.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3nmvezmoe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3qrtqwich.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ixgyvxzd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hxidhlhh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3cxlwucxw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iihvrjhx.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3pmgtrfcu.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bavdyauy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3tmhdeild.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kkoudtve.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kaidfkmm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hckrfaot.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3pctupumk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3rbmrbnsu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yroaghri.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3shyrfhhm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mjqdxmiu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ipjgfoxp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3qpcwhrpf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3sgiolvbi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3goxbjgcw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zcctinks.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3wtakzrql.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3yhdvaldy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bmgwdshp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jqylskdj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3uwphfbtz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xizxkmke.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3nupifyhw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3xuaxdgfu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3wfrjixni.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3nyvrrrxq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yhccqukw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3snewgmho.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iqkufmtl.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3okpjwlto.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3nghbqpvb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3shywejft.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zbvwwimx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3etrzaeic.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yljzfrip.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rziovfrr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3eodopyaf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gskzfkxr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tjcxejhp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3vsprfyyk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3jylmdetl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3hnvzsnpd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3uqoheztz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tpnlafeg.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jmbjkaiw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3spnpvjwm.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ekhzcebt.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ofxihgsf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nbjlnozw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3kpkdoebn.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eymsizpo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3xhcilixn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3epjrguno.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ofddiqeu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vxucjacx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3oeeddvhg.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3cstffmuz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3grbxslem.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ydfiocvb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ajsxjmxb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3wcyrsgou.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uflpecoh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mralupyd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3qnrisris.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3auisagqg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3hgoscqda.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ypqpcopa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ilatpojw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ojpcasfg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3htwtrjns.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gsjvvyre.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3szdcshct.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gbjymlbo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3nbwsxgox.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3uqhdlszx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vqrhjskp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pnzvqujy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3emovbjvn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3kjgtwjit.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yozkniyx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ygmrrxxf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qloupmpk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3cokeriab.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ecmzjqhb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ygcfkyng.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mbvxtqcn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3owhqnvip.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3oqaqeibu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ldiylnpg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3agquvoyk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3eneppwwf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dibvqwgk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wcmpwblj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3qmrntopv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3sjcejbmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwamrcyb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qsezkhrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xsvqgyov.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3wtizwwim.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3vgmrfsda.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3akhfdacn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3bypqresg.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3chwvoaff.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3tvpqhdhe.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ikpxeule.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3jhydulie.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3xpuuvvrc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3miuhewrr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3mxdwnzzp.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jimtmwsd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ktdgxkma.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3fbzxhsya.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3sszdungc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3zblponef.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3nmgvoiwd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ltrjxgfm.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3dffeqxyr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3iyibbjdx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3hahkabiv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3prjxqwiv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3erbmexxq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jppaqkly.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ydenbxyj.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3dtknqcxh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3jhlsbmmw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3aodpuoyg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3anvhmwua.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ptrmddpv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3bitfiveo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3mtkgnqnr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3bvckdkzr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3arngupqv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3kxoqsdwa.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uxljbogl.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xgmkauoj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3hrgafuic.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3zhpujprx.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3alyjmmfn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3aytzcrcw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3elhwlumo.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ggtakqne.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3zvmhosdf.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3yldxmupt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3bwvzmjsb.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3cbpfuboh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bsclblra.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3hxxanjrp.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3jtdoefxi.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3kddtzrly.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3fjfnpulz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3vyacknkg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3nwkgrvbf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3bmbbpwqx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3pmgosamn.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3obtebtwc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3tylgygkw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3nztjthia.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zricarqx.html


<!-- 参考信息 -->