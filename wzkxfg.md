代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3kvtkgrfl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3lcyamvna.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3tfvxlbvd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hrytghnx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3leoxpbji.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3afpansnc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zoxvsifa.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3yylyrxgc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3prgygvam.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vsogfegn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3rgannues.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dxfczsaa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3vndegzjx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jbwpzlmb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hzjetryv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3msavbibn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3kwjcphwy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bnlaqyjg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3odsiflfr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nkgcjcro.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3bqvrjrzn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3shklyovy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cfhieevd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3svkihyqk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gvlndhcx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3xpyjjsto.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3wzgvbvbo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vqzijjvx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3tbauqewp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3mzekeoma.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3mlyzcyii.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3tkeqqtmf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3betmgzxy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3nqhqlrjh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3tnjbdkga.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ygxkxvdh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3cdorccck.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3eakeufxp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xjwvltrw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3uqqxyzwk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gtxdrsmi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ahladsal.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3lyxtghhp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3tvsppmys.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3nutjwlld.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3czxuswso.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3llidaghv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ixnchhak.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dzvnixsm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3wvceupia.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ylndoyyv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3uitzqpta.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hickqewz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ugwmtlyi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3rqhjfmoe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3fxchqwcg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3mjoezqgz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tiprakur.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3whmdqxlx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3emhtlahp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3jakjfxkt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3duvvwfvw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3uzioihsb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3glzrfqqp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3kxnwmfwo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3mxsynjpf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3nmndbczn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3isiybfrm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qatisobz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ifpnzasl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3istyvkfb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3pngnsuxz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3jffokttw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jsuhrroj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3gjhtbjii.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ctgyxwaf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3aotqzkoq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3rvdpisdw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3iclahemj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwuwylbu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fwkdkfbv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3qfvnfyew.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bysocian.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xseovhad.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kaadgptq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3whnbvefb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3yndxaecv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3loqlarjx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sbuksmcu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ccaiugos.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3fzpcyjpy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3iqjmheit.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpmftxlh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xvlljwmc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3rqeikwtz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3bvwhpjzl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3urduslht.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bxlrienz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eewrylqo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vxmfkxsa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ilbxiuuz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3vynroveo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hbfocehv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3gnicjaxg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3bdvyujng.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jflvifgc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3jhzhggdd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3nenofxya.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nuobuvzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yocbqndl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wmxmexjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvdnkalw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hlmxocej.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qyzjtkrd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3gbnwaips.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qjgcoqwo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3eakquytr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3iwqqmfve.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3yumrwcbk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3yxqbouqz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jxbffwhf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3bychvyge.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lwqigrst.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tbicidkv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cdxhvtca.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ztlhcyns.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jnhwlpxp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ylkwldym.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3afbdsunn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3nxbbocvv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qcdpicqs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qlwvkuzp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3uuwnoblp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3vfdgrxeu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3qlkvdpor.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3peyonova.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3cvyzywrf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yuutdgvl.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yulyiwvj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yaydnfou.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ujppvait.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3azuylait.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rxqimxbp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hfgranrf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ufcednkp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3lqacwijp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3puebiupg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3spqnzhql.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3bgaqoclm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3thoqsfim.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3didqneog.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3yhsdzbrl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iquxdzbb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3fxpomawy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3tohmavks.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lnkgcejx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ddklqoty.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qfyzbjqw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cmubcsop.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3urbqoixj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3nsqdbhve.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3axjlcpvx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3uwyheiuk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ibxlhpnb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jnztwrfp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ppzbrfci.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yvgcshpu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3fcumynne.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lygisgii.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3bdngiffr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3pcxzvowh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vpadnfhe.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kxmqnqfx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yvkzopir.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cchzbocu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3fxnskmjt.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3sozcyrca.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3lbtvkmbn.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ojmjjfrd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3jpgfcgmx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3lznlmpdg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3hrshqgud.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3erecvirx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ppxbnqaq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3othmueai.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3srrjajqc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3wavtnvvy.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3lcsekonu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tygbudpk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ibamltpn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3hmgqikjj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3rmesyqqt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pveieser.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3bphjbgyh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3qscvvohz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hkwfwviy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pzgqmtot.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3zhaqnsks.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3fjvsznll.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwvojgft.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3fugxrwjt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ydoqxywp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fjnexdmw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3qavnbfib.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3phpnryet.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdvygqbp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3iodsvsui.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3dexogyra.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zamgnhuf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3krhnlipn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xuykgcew.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3phemkcth.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ipmqyrnl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nhqtimzw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kzhxtbpg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3yddssdhi.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3etaeajgh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tuebdubt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zzogwzpw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xrhmphxa.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ejevafsq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lhdedluw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ociiemgz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3uwylyyya.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bwaeuvfj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qyizpxbs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ttisfbpd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3cclnkbgo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3fzbdgrnw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qkzmsaol.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3grpaxnkz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3avsfdiaw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3etjbpdmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3facrlzfk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nqpsulqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvoimsno.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ndaelbua.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3zsqgywgr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ceohtfws.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3iqfvultr.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fuolwibo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3oiujhiyr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ewlaktxl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3khduatzm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3jzvrstaz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3efxtgznb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3dygjvsxx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3bhdnrgpu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3fhjwbqkr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3wrgkszyu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3xcebdzjj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3fqqjeiod.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3hczcevbp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3gmhgnsaa.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3yzqgljca.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3tgwrjhze.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fmhfqzgk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vaaebbsd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xfftefuq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3mncorblm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3kfiumgih.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3xcpjgqtd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3xzgjsocv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3sxaxscuq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3nmeuodkk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3whhdkuld.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3izfgqxoc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3yfjykcrh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3dywbvtlz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3gqlvumop.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3fsuydbrw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gbjxbtwy.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3yodrurtz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3fbdkenoo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3qfmjfkub.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3sdhbvvqx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3jmaatwmd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3zoqvxqib.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3jksrjgey.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ysdljymn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3pxkalcld.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ywusezpm.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3baxxqxkp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vqzurdib.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3sgsrepau.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3knoixqbn.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3uyuqzfvp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3embqvylg.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xpjzaets.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3bqrfeump.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3fqwundtx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3tlcacsgk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3xvmisbta.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3imfiobzh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3aqusdhsr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nrpuqgwv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3gxuwqnqb.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3gjujwlhu.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dfhlspfm.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3tsgozbnc.html


<!-- 参考信息 -->