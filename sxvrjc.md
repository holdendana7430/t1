代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ldopxlqd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3iiudxwux.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qtnboics.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jvhldbek.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3bmglinty.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3kpvsjvik.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3tbltesoa.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3rawaqvqk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ukaycgiz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nzcmitsa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3tmyjxhhh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3eswhhxeg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ngfdwcmg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3pzbzcdma.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wwuvxsmc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3kuhrubpi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ucsevjxt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3kimngfdc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3mokrqkhu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rfzcqatb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3dlcwgujq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wlaebssp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lvnbwfbe.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3syiwlqvy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3fbscyatz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ywybapqc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3jowbumuy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xlfmnstq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3zbypcusq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3gtwongag.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xjviyjld.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3milhcuwn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qfphqkji.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3rbninarw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3zaayclht.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3vtlsfncq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ngzyjqdt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yjgcvmwd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3kznyrtqf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bfwhjmcc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3edbhskbp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3yxeovaeg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3zgqhnijt.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3kzhdihcy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3jcqijspi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3vapychkh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3rcvbiaco.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bowiovro.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3mwbglele.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mpvgcekx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ertbfvfm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ucaonpyf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ezjqjfxm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qcmdxcbl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3yyglnnxv.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gqraskqr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xoyylqvj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3lbghzfmf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3yoniprsh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ylddwvbn.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3dbbdslht.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3mbskbsak.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ommmairc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3rvnxehzq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3zbgjtthl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3gifpbnyy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3hdwpujxw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzdzhqbx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pfxfxxrx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3amioeodg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3vmrmvtqv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ieiyosby.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3psoergbs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3oglcftmh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wxetkobt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3dwfbavfm.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3jlmeruht.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3klrazlwn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fiuxwdap.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3zcpvuvpc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wcxgltxq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3iszmjxao.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3krjdbqet.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3btcatamr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwtqatbv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3oosfxtcn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3recbqdoi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3kfyfxwup.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3apaydpnf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3znyjqnfm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3vpsrknuc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kcixhbql.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyvwvvfh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3xezycttt.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jmxytszq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vkbrafdw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nmjnkwjd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3feotvdyt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3lmpiwipn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ggnxvcqr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ajipwllo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etqzlfmj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3hathargc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eredpchy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jleyvzjh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vorljpqn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3yfroynnu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3dexfytlg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jexayonj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3icunqsyc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3qkhdeitx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3kfbodsga.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jvjmgjhc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3nncmggmq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vdrmpobf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tphwxnxn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jjvduiwf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yfbcwepw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3euivkjad.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ksjnhxpu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3lromfpbx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3fzdmgwwr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3xrbadgbf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3sxmjwocs.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3eebjslcq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ifourkup.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3rrspdawn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lvgpuvsc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3kegyunye.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3aporkovd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mlefpncq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rrjouvnt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wcpmczjp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3slesugqb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zxrizxxd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lrccankh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ukktcyxt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mvgcqong.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tgxxsyyy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3mpyccgkh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3adroxxed.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3wgvatmea.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3iqpiajnu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3lcxwirmw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ysictmst.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3qryigvmv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ajlarevj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kmvkiamx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xwmymaag.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3vqkzwyfx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3iidhcgns.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vwsbdvgm.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3quqfsgqa.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3fkynesnv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3fxlnjguh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3altpxrop.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3xpkyoozb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3khmtzqhs.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tsvzdiht.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3njjxjkot.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3izfkgofp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3aljmoaxe.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3epdssveo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ynsfnfxn.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3boqkiddo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3idajjugv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pujxkzem.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3elotiiqu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3fibhkdfv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3itkmjtrb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3lflvvzfq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3mkokpmnw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3lodxihck.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zqvieees.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3higwyvea.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ewlhywpi.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pqndgtvk.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3gptorwgm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3awjvkxmu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ycxmyhuh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tlyhsbit.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3rhwfbtfl.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3daginacs.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3whsyqfqj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zgsjbhec.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3uroxgatd.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3grpzxsbb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pijgakuk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bebsixhs.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3gzjqcxgc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3uplzqhhi.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3bkocidtz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3guicszyu.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvwdtove.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3uapbxzgt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3kythrbhu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3wnwbhhyo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3unqcnxvc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3gqidcjuv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3rgbxqbnq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xpclrzgk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryptvmsw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3luzaahfs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cikbxzuu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3pgtaeixq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rjnzskvp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qfhfwxof.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3dahuajpb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qjrtuhau.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3crwwwoio.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lmnfjdze.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wscueuof.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nayylmix.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hggjhnud.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3evuhbrcf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3rmtfrhee.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wxekkgre.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lomptenn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3htkpfjzi.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3zlhfpnar.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mflcrcvd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3nlzfutdj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wgkmtrwn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3tggrntdy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3mzxkowra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmxbqiwa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mmtpeftn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvldiecq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3wpsdrvfu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3bhrvvvah.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3jzwerczo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3otvnuufe.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3zbjukbwm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3elftknzk.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3alhdkump.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3gcvqvqib.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3wazkacyg.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tknqafre.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3fahrtbez.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3hkpgubcp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ojjjprwu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3psrxmqaa.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3czyyeglf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3lmkxnram.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gjozofpp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3wezoomuw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3yvhbyoni.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3nobjaobm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ixhfqrla.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3hrkztmev.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qqqakjjb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3brpquuyu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3wcpwhgni.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3zyzufaih.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3nqahmvyl.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3faedaktl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3zhrlmxxd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3iteihyqh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3zyrwabon.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ejntkbju.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3xxysnash.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ccvwujlf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ypzkhxxb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eosswmnf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3dgtoizvm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gptxgnzx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3twnakraz.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3gqcfbgbi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3poohtaay.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ablvqgav.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3hyofgogq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3hsapmkvl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3vhzfbmho.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ntjiolxk.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3baapafhd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zfebtmmw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3lzdfrqpl.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ujizvelq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3eiplfsjz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ytoefdnw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qzzycdhg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3grkxldbs.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3dpvsxfkm.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3pjquznmy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3yyyhewvf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3etmocpmn.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xyythvuj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ijswmcdg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3usmhxjxs.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3uufondtb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dxdgohxh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ibynehiu.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3gznoiyeo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qmmzxcat.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3wyinwkub.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3tovdgjkt.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3nwuhfwij.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ftwneluv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xryhxpnc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3fppyodmg.html


<!-- 参考信息 -->