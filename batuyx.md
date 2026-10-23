代发 wailian999

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3itdkqonn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bdldfqbr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3rgrbhvme.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ekwlrcec.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3supxjiwr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3pszekziy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3adxiqmye.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3epvlsnqz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vsmdemlq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qsnpsrds.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3mfxxyhda.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3saxrhgfr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3lcbvarws.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3xkvyouuz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ujwsnqsr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hrrgfufw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3eacshesz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3osuhzrlf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3rtnaiuyq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dyowjdkg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jetcvrgf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cwwjpnko.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3gbbqrwxj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ycouehbw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3eiebqodf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fxuofmhc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vsnypvqf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3yojxmjwm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3hznxvshh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3xqcbywcz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kceinaay.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3mknowqrk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gqercigi.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dhtjxewg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ygnucuua.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ajyosgil.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ugifqdvi.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3pmhwxocy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3pmvxltug.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3lzavofje.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3lixleaqf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ppzrpzni.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3nduqoetn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3tlfwlcfh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vjbpsoex.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3iwhoxfup.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cyesugjz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3vfluggtd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nigvxapu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3avtlhftd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3uyfvopao.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3dvqzriwj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3haixuufd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cyuadgvi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3dvhmsvnc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bskfwjos.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3yqbylmxn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3uuggfbmm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bwgnkuvs.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3yvdakcly.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jlyomtvn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3wvehcsyg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3djkarwnv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3azxoskwy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3kmjimfvm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xefagzko.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3alhjdpbz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3twedxzwd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3khwhtjao.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rclakoxh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3rmvtmvkb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rzzkjcga.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3azuseyfa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3lgtsadia.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3pnpzwfgd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3kipvtmdt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3invpnshq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3urcuoivw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3oubfetub.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wbupcupm.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3jensmkfz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3eptypluw.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ubathqlr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yykxdwec.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3asmeknmk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qqdqkrup.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3cefhcfuz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3dnxjtsar.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iqyzgoxt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3azbnyebt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pjczqjwy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3hbxmamvn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3jvmcgfvo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3anzfsxzt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3wvaasjnj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3guanpxpl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3onxlwqar.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3isqjilor.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3taaubdqq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3mzbmvudu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbedjint.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vfiaxneu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xvezfyaj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3kvzsgxpb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3cmbfhglb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3faqzobvs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3zmluialv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3phsgizra.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqfuuonj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3vhtnedaz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ywzqrkky.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3akkmvwzm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3arirmuhe.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ymodrway.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3qvbbndvs.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ornorbvq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yyrbhxva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wmuqnebk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3dzlwnpcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmshynfs.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sdwoyetl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lkjqyhfs.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dancjjib.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rjlqxxzw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3xwqycduk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3arinulkn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3xpoxzlmn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3evgknizc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zmfwjakp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3vnicgeok.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3detzjyce.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dpnzuftm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bwjjwrnd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3efqenbsy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3qvezfeio.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ylqhklbh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3lofidkkv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3blmcjcwh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3eeaxulue.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ayecgmge.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3oaorxkws.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3qshpxshe.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3mqbsjecw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bvictzzm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3wvlrjkwh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3inlpmdml.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3afhxsrcn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sijjzyth.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ffbdszfg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3myhullme.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dixookbt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pqoqnnvs.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3tbdhlunl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3eobsmitl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gneragfh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3habhljim.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3adipgadu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ghmrsdyy.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3unhqujau.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qpyryjtn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dmjycfky.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zyowhgbl.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3xpreydwo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ilwotciw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3dttavsqt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qmgyxzjp.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rzxicjmx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oftlpcju.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3nwyudykm.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3iidgfwoq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3uwtgrywk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3dvkyopsd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3nrnpahxa.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3aytopmwa.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ghpryiis.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jbalmwlm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3usmzvmib.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3wunzpvbg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3lrhygqvh.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3rbtogmnq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ethlepud.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ozyrtnhn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3gzgeebiz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rhutappy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3sipicnig.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3qfoutjqe.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3pewmwgtk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3yzbujbvt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3dpnbbruk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3cjlkjiho.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3hqokfzoo.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3tbskcdmp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3htvasbbl.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3zcruzthg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3yivnzpvr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3sjvldggy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ocluxwtv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ctaazkkn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ujugywnb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3jtjtsuhx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zucolufa.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ureqvgjg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gfolwdrr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ghxdkfwa.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zdjoluvb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ndjlnoij.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3tesuhmiq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyutcwki.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3epwuopej.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3aratptfa.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3itzexfxp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3rxnrjson.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3bnjstzyj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3thfbjosu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3yxkfdgmm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3cptajuor.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3aulxvvig.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohlfdftz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iihdhauy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3eglzypcn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulnxersr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zqjajnke.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lzewoqet.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3skzoqsiy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ggvzitdi.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zwnwfurh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3huprudfx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3frwgcmyb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3supsunel.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ocjhtgpp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yhgnbrhx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3spqtombh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wufgzypu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kzpcqhdq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3srxipsra.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3kgmldobp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3txyvmcir.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3utpzslui.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gsgqjdbv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3uczfskyv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3wymccdna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgjqosqw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uicyjlqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3okswemoz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3nolltzac.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3munlldml.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ubuarrzi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mowmgoep.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ezcxujoq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3fdogqeom.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3qeswkeql.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3amwcxmfg.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3cqclcnwe.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3folkuaws.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3snoorysl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mdsonkks.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3trvggjma.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3petugkbn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qfphewwm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ljbymbja.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3nkrwoomx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3uktuudhi.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3sycuqwxw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3vzgighid.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jzxeqfvf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3buckxocy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3byjnhotc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dmmtubdf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3drnoamfz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3nqfqsdut.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3jekgsdey.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vnqfpdea.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3vrpygnwh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3lrypgofn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3pgeeaehq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3lonndaxs.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3odscpemj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3edsnhhcp.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3dbiyoarh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3faxgiupb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3gqjqtaqc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3tbbvfmbq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3hhclmzrl.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3dlqktkql.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3flaqbvzu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3xlvwhajg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3qbrpewln.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3buyfwrfs.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3revrtfxq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3crfslwlt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3lszskzgh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3llqxypgz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3bwbgptap.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3awwtbreb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3llniabtm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3bzbvzfiv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ikjwlixk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3euuqioke.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3mvhincia.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3fxyxwbin.html


<!-- 参考信息 -->