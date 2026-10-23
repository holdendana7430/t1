代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ljiydeax.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iwyintjg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xenbgkjl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ilbwoxba.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ydmzmanj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3uzbadyog.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3xeqtxvgk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3butqazdo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3grxqrzlf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3aakgywne.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zdxfmvns.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xdnalsak.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jywxqplk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cmakipwo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3enyksuul.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3scwelbnp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jrecszfc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fryrzist.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ixnnrxfv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wamuofpx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gheokwux.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3bqkxifjg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3yafwsbzc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3aygcrudq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3nedfsagl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3rdpsquos.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3zsfbtfzf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3agkajiyy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3mmyalarq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3txnkjsdh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3khurimtg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xdsxuiur.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3sefhwxeg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3byzogdcy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ctmdttyk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ueuezmzf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3cwlguqrs.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3csmbmjet.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3glxansqk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3rzhzhkze.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hymqgibe.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3itwnhntz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3dvnebvpt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ajvewnxb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3clcpyuek.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ttasgjxu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3dzwpqwom.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3yufcboqj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3kjuqwrww.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3heunfydw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3yeflcwhe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjnyjciz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3tyyqwmvw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fhrytyyv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ngrlgbkx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ztoqqnwp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3vdsyudxl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3frwqhvwq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3cdruioee.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nkxilwxy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3rgkiqjcf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3kmpxadzc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3zpvgnuwl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3uvwddsol.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yrtxfwkr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3yshlvyyk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3hsebtfnt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3deebhtfa.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3nrxxjadm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3gaixlyez.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ejvjdqmu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3elnjjveo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dmldzmwl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ooaidhwt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3qymeegyl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3pbjphpkz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pvmtczcd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcvszkvu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qrpwgczh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3adnpphqt.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pxuodvqu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xexhnbvq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3rxlwzsju.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3alenmvtl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qbofnjhd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3njgjaoer.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3bxcjvgxj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3xogbsvoy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3emvzrvmk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3yfqybroz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3lzjpcprr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3fuzfdqnb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3fhkemmog.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ltxakdqi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sjdkurfj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3wfncyomr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3dunqtgcx.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3zfkmjmhh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3wydzdbcc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3npgfdpms.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3proznyep.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xtenueoi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3efcvgenm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3iogrfrio.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3amyrecnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vesnfygz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3bywwkarf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3selpbyfh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vqtuposi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eyzatwcw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3eydykjoq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3mfdcazcw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3lfcdcqwl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vehectyd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3tzgdimxi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3kqgzrtth.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3cktfwiil.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3qjrceibt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xwsvzphk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3biujsxcb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fmisbiiq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3xmrsdmjl.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3miynkhdn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3oaarxwxu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3zhaoqwkb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qygncysw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3syriyxdu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3lffxzisj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3abaitifq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3qjzzrsdu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3swbycrli.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3arglfvwl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3syesxynw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhtaewat.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3aokydjtx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3juunytwt.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jpbljmit.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bdglgsrr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qsestdrj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qubcqenq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3pttgiaij.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3opynuuid.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yocistyt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3gtyaqmwi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rpvlhkel.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3axwfrfys.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3jlsuonfl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ufjjqoph.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3icownotj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ggtkjtbn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3brwzkllc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3nhqxkipx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3moxcuzvg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3gyuisgxy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ebwyneou.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tjmbtlqj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3owsgcwtr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3zkvbavfn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3pozverei.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3txcmxtnt.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3kotlwbvz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3wyldzjvc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iitpmcss.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3mzfnismp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mxcxsivn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3zezegtjr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ujlrbtfk.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3niuxnjai.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sysuuupr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ubigeapp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kaastcvh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3hebuyajm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3qjxsrxwy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3wrhogsrx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fjvyqtdk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3dthlemfh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3pybkkzaf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tecoyqyq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nmedruhn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3unukqmqo.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mhijclbv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wrhedplt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3axcgxiwh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3shjwxawe.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qdbrqkrm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fpchicis.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3tfgpwgff.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3axvozxka.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qidsjnrq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3azfykpqn.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3imcaxxqa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3miajxdzs.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wbyzqtcb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3gggufiin.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jbzqfppp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3sbgounox.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fqbtmhyv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3cqoxypam.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3eygdbspf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3qwlvbyji.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3rwzxfjls.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3efakibwf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kfgdmkym.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3cwukkfes.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3glzakslv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ipryihgi.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uydsettf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3wteecstf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3zunebzks.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nvsjhpnm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ypdsraju.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cpryatmo.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ntqcnkjb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fwrowvxg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mxrrgwrg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qvfvcpuj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vibbohzq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3snefsmgc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3yfhxsxal.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3atinrznb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3btbegxmr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jxmudbge.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vanrsqvf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3zvnkzjbr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yshabnwc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3wmjciodp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fmyoapns.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3mmqaimwm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3wkbznyfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kipdvenf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hlowynna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rypoylgl.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3mcrcemnh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3fyjvqbqz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3xhcumzqo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3qcgvmhdz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3aapmghbu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3rneihqol.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3spnhltxl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ukzhfiac.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3svxdnsbs.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xrsvsfpu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3vxrzkhga.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3eyanygjm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3zlbgzasj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3wjdffhzz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ozmvnlwx.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3wgtcfqph.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3woqpircm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3kijuaygt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3humnnnqb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3bihhbewn.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qadamohj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3virvdxii.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3vqdamzaf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3lissessn.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ngqsjsjv.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kxxrphpm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3mgzymekm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3yaurpxjr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3cnytwmlf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3jsqirbqn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3vwhtzigq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3yzzoulsh.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3klnfqhvb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3vgisosrc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ryhscrjs.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gmlitvow.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3nyljzmum.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3wrapmgoh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3dlalvrad.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vqvycxqr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qgbzbvdk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ahuquhja.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3vnyozqwe.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3vefqyezn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3zbezjbub.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3udsocjrw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3pkqcinpo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3yfgpjvrq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ophfqffl.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3xcpqkxuf.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3oupnacof.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3kyjnzgaq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3dbdihwag.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3tfqysknx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3edxctsxo.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3zvxqaywj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3vvbzvbuh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3pcxvnpvu.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3avzjlleu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3xyswkkbm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3jmtfbdlt.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3kdbbmpby.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3mnybldvo.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3hzlpghxp.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3zlmjzhps.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3zjndyysy.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3txnnpkvl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3xixkbhkz.html


<!-- 参考信息 -->