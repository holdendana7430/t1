代发 wailian999

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wbhapohc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3klxpmtwf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3cwaohnad.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3smrahvuu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3mqnbmcdl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3xynwaskl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3yqvwkzvu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3pcniowdd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3dyfniuwg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3jnvccmxl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3fqgjoyny.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ruzhtbit.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ryqktolu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zviebfjq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bpauydxc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3mwpewwey.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3opunsaop.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3nmoexbeo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ounszkqb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3sbqaqgro.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ezfrsnhs.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3iqhixlzv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3zbogxibt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3kwsxmufj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qwlggsuu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3arobvxmk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rorhyogo.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ltayycey.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3vvjbhlqt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3umzzpywh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zgwazqtn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3bfaggzmu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qiwpbqxl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3qelkoiri.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3zkzlmycn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ipihamsz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ipomjbod.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bhljtudm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3oumqfgqc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3tszxbzxk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3wzzjxsak.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3nqqmkngz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3bygatwkv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3nwejwmho.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3djwvporn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jwugkfvj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pygamjkq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3jmepbjkd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wfstfhkd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ykdoxxcq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3dxakwmrn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3wfsrxota.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dstpiypd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bxqarbsl.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3akotsrij.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dnbeptpt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3fddulqmi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3spsuimjd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jeuwlezt.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3crboojam.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ystakgfc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dnfuwftb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3fexhowxh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3fcpmcxds.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3nymghxyw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cycjxtgo.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xielpwcu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jexnmxwi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3myddindu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xiadltxb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3hbsfgaxt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3junpoolp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3jlkkwhep.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qslfhgcn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3zhtgusgw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3lxflkwin.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jtivshey.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ksahhsds.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3mbnesvtu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3nvzzibab.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3eacqdose.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xfgztszq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3javipptt.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3lqensmzp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mcaokseu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3qcyyhggq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3wxonowfb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dymfkuqi.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ymvcrvzx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3uffmyuou.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ugyhiafx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3kqfagpai.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dplzmgak.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcpipjxu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3neefrpjj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3rbhxkryc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3buodpqnv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jnsvcahh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3dnxovapy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3thzaqgzo.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmvanaah.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3qqdizhcy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3tprvfbvs.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3lnrdrcwy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ccjitkka.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3yyckaloc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3gesqiqlv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3kahtackr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqboctqg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3krfajlcf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3pkdyhgqt.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3jzszcvdo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jdrexmjp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3aavggdty.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3eusgjhcv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zslumbet.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3adivoqpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3goeqprss.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nlzydajx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3satqibbe.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bpmazmkm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3omsxyapb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3krqqgdoq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ciyznukv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vqxibdwf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3omzluqhm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3uivsmrsc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hmjirkyj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3nsqgambh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3tjloirsn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pypynmko.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3eonshpvc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vdquoodm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3aovqinhz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3jdpqvicx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wazabnid.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3cmkcoohv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3jugbauqz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ofiaqxjg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3duozxbtv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3sznivlyl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3brcxcech.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3qaumsgrd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3baosthyj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ltmdaldi.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxdmsaap.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3tdnwtfca.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3suwxakhy.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3nnvtyzwq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qmpbdiku.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ycoqzyud.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cydvesnx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3citgcubh.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ywfivdkb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lstlmowo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3jjnfitvo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3pnyjpctd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3qbkzcntp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3wdseqlzu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3xishnzad.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mcuevpam.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3qeviwqou.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3nkpzlzrr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3faplvfke.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qvzyooix.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nslabmkk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mlfmxhjz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kbequhuz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3libhdhwz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3xunneuht.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3soaqpklw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3assnvezs.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wqfcdsov.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3uikfpigx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qqfdftnt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3gghbwmza.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3noctytsv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3kfdxveqk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3gqrsxvfy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3skkmlrqy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cjxomsxn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mdjkmadn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3rxbsqbac.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gnloourx.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ufxexczr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ghcfqjmv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3lstyqmeo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3czrvynnf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3rlxpnmls.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3qlsosbty.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qxktwpid.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3sglonqxf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hcvvebai.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wicdablc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jkeuncih.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3iglshfab.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3livzlyqx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3xtcxdjbl.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3sceizors.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3rctjsmcn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3egdpherj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3wagerrym.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3pdnxxsii.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ocyejxkp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nlajenrb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3poghybks.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3yzyekvxz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjaizewt.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bifvbiip.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3gtsseswi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3tpomucle.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3avafxxum.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3vqrdxuax.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3iwtkfkuh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3bhbqzoyg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3wigcjufp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3euzomyiq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ciozhlsf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ynevinbu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3rbuzhkjx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3hahrzjnd.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3exqjvxgp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yyjjzlnc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3osxyoxjw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kuxmmvzh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hggvgxrt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3blovajru.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zanjumie.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aeufwhht.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3izxvzxbw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3aooflbeo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3skazqjyf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3oylsdekv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jovqmnke.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ilgijert.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3vjbvvptr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3droyxjkl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3xuirgken.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dsogcjkn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3svjjzefz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3zvecvrcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awwfgfsp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3licbenqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ohrdxpso.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3nmfokgpc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3strrcggm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3isbzwygi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3kgrziptg.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3kdlqgewv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3yczxithh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3czekhelo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3grjfjsxv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3xscsojjy.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3floeqtyw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3eftskzye.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ybgynral.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3tajxxhae.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3uzmijivs.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3nyylvkqa.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ublfqwjf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3vwpomwji.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3zysttvzg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ekvojdkg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3wqyfsbgs.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3osuuotpe.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3qtketprs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3jkglkcxs.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zdmtajlo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3novecosb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3eululotv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3dtffbqxe.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3iyzejyhk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3gijcgoia.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3uhgrvhwu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3yltgbdta.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hafrgmfx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3lfuggwqm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3osysrngz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3pmefutod.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3aerypbfy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3gyvrwjni.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3bfszrwqz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3rdpcloyg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3tzrlfpjo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3jdlzmmvu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3gdcqmylt.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3fnebothb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3flldsnxw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3unadqwzc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3tlxpabqz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3qbfcuqqc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wkygbyfy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3aqjlhefq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ozfvhcfv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3qzdgukbc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3nyalbjyi.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ljfuiomg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3czaoqfho.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3bdgttsmc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3uszraxpx.html


<!-- 参考信息 -->