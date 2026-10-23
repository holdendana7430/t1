代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jsjctnmu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3umukrojl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tnsmghqs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3opzgblgq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3waxeccwt.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3alprtrrd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3iotmjfpq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qnvmnnqr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jrydbqym.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gmodwtmz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3cpaygcnh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3kqrzyokc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3tosgmglm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3krxwbnni.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ojkkxexd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3swetetus.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3qgwwgtws.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3lucvbbza.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lljfeobk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ibiledxm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mqbbdnii.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3nvdvnkdh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ojyyxqiu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gwkevbti.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qgvzseik.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3owkbvvjf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fcqkfkzl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3vnmkcpwn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hltdwouo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pmlzpbfz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3gnxatxnw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3lpbfmxex.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3hgimsoko.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3wqnqhruq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tnkcwucb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3usppsueq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ubsbxmdn.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3phzhdmic.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3afdivigy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3cixvbjyn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3jtfjsydb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ycbezvsj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3aoyztrwg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vhukgdle.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ivtzaeoq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiqqsceo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hhcaxspc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3yyauhdie.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ejucixnh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3agmovpnt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3zhjjegjw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xcvvkrrb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3fplaiyeo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yjpouvwj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3lletucom.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nlnjuwbp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3kafoyslm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3moicoork.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3vnosfqbe.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wrzaarbv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3gsyuolbz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vafscjti.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3gvdqoedr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3xmbhchkp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3kilmlvav.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3tocsvfgp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jsurzczz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3lphphsul.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3mnhakuyh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3driegobe.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3picnerjn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3wrdbccau.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3iaissysp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qkzzjzso.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3undmevuw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3kppnqhhd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3yidjyxhy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xlgbosku.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gqesmdis.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3vsiybdnv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yfmwawax.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kbzyuekh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pvtbnpxu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3fyazaxcn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sieeccrp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nlikbdox.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rzmboful.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3bdzgpzcd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3rkbjcqqt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3fjhhwdlb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3qjznlwej.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3xdpluucs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3czavulnw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3tlxjlgid.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3wgmxrvjd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3rdhevwhf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vetkjwjt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3zizaudch.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ntvrmops.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mgjrlmmq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3kmtoxpnm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3jwglalom.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3hefdwuqw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3vivozkpa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rprnhkuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hpbxvyct.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jntebjan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhqpfizm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kbgxpdez.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dkhrepyv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3thormsll.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3nmxojcll.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3higfbytr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3npgrulvo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3xnvoxdtc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qklwkeft.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3fkhhjtbj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ctaqussm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3uhxnlxcr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wswllilm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ttfchops.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3sudsntss.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3rotteocd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xcikuiqn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3vmdpdtvy.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3kipvmxoi.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fxittecp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xoajbafc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3xjppuzkp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ayalsdvq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3tizsbuul.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jfvmrpaj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rkwlujiz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iwvodldb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ueznbbcf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jazssddc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3dnxokscg.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bmfuxkas.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bsgsstqs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uzssmkxv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qxwtvstd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fjyuodoq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tgwpvzdk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3eisrssss.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bppqkqld.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3dlyxihnm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ygohbjqm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3uaxfuwny.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3tnkngmcr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3bqfyjjts.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3nlfsgfbc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wvwvbxch.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3maqbjvbg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nokillui.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xajuahjr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aqljchdy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3pexaxljp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3xhfheveh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3cvtxbujb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rcaixvrg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ladacubg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3sbennvgb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3pihbopwk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3gypgbwqy.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3mdneyorc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3aeezzapv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3qyasmahc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3esknjoxe.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ulcsxnse.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fbmeysns.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3clqwjdkh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3kkesuxys.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3dufkektv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3auwiofuw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3uucjhcvc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ereonges.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3dvswqvbo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3mmqgbbyg.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lruideid.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zrpysjez.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fupgqoei.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3smfvhqok.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3dlglhjdb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ougibcaj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qwgsyrwq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3glwhilgp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ohouddlv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3lbqlcbss.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xywnynbd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ovwuyysl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3dsxalbzv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3jbvdulgq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tmaspcst.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3pbvgdebt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wbdhvlvu.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmhalkvx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ohwrroio.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3orkahars.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3aelvyirk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihczhzvh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3dskybeda.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3czekcekq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vkxcqlxz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3lxgigbay.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3mxrgslkd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfshkaly.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3srhsesvs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3xefvshke.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3mkkblumc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dnybtjhd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3epobeyrq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ieicalre.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ukjzgghi.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pxnqxefs.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3crvwufny.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lfmbtsgd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lyxjocjp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gcivthzy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3swiqkjyy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3qvtebbuf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vodlcdxh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ibugclnd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3tugrdryy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3pfmiqipp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ajiymmvu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nqsudajk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ygalasxo.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3cmnkrhkh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fqqmmcmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkkwuddl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3znlfljyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yuymwxgh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3jrqlqfxg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3xxwesjbn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3qguacgpb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gdosnuwk.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3uizuepcm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ftgiibmm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3orokuuem.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3hxzgznog.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3xzmpxkev.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fgpgmlso.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zdkhhals.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3maptfgvb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3yllnkpzx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3cwmkfooi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3gskjvoah.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3muwbbumz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3hflbmrxs.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3bjlunmsd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ztnqekqm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3bdgfougk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3kcgszqwl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3sthxwdbl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3izcfpeoz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ummuupjn.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3yyyaktkr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3blvjjtzd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3vdkiggyq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3kntwqkzu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3jdicoizl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3jvktdnav.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3tgikfkek.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hteyqnqy.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3zldgjokw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3qcgaoksa.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3eeftrfdh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3pxidevqg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3bzvyvgfk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3dtnhujlk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3zddnuyew.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3fqyzgcsa.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3oewqrnwk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3bscvfwdl.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3bcpwqxif.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3fuzbjggd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3sywxnjsf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3etemowpd.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3kcidpvqd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ofilfrlf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3psbmuqnu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3mbzwvfax.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3igwkdomc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3hskonplu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3yuswogtj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3zyocfmyj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3dmongvzc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3natxowrn.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3qdntagsm.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3qcejpbbr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3wqauohsi.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uxcpltts.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3gknczeki.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3bfrapina.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dixwxeva.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3qtsyydrc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3fiuntrvp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3nimhodxl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ldreccka.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3nsoqaywx.html


<!-- 参考信息 -->