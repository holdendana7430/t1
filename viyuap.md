代发 wailian999

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2szaldxrp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rmpxumba.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2jmknilwb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2nnibudse.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2kznqtajh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2kkxxmuyb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2mkyzpvcl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2xpsusvca.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ficaokug.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2pdlbisyq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2iccmnkgy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2udlizxjm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2qjwzunvy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2clpdquxd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uuopfwwq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ppwhmmmn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zzsitdhc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2zdwmeznl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2dnbbugpq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lypgeifm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2eftuaygm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2vrrnfwgs.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2erugffld.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2nodhiuom.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2scofrjgi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lgotyede.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jlbgljfi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wwjnqgbw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2vkmqlitx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jwenazik.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mfzindzp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2yqcvxccp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pnxtzwol.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2skajuecd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2jlpkwswg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nlkzgxyl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qjvpbuah.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2yclzrlaw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2oqtepvwc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2batzaoif.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2elqdqjsv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2avypjkpk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2dpltjqik.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2mqkhokcr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kqavdkma.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2fsqzybhb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fsodvgcw.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2upwjnshs.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lsculsmg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2gzcxvxbh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2hmybvauv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2rhiejoio.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wbhkvghd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2wipyvlfj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2rsrlmbfk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mgggeztt.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2mpurbswt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2noggsasz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2nbibeeyz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2mqnwlhjk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2wyezegin.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pplhltgy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gurxozwk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hxhyacwj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ucojtssk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wabkiicl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2kainyuei.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yoydxjic.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2geeymgms.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2coytpugn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ytqvzoyn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ybxtzsem.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2slalxtxg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2osilyvfl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2aohxigwe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zqpsjskk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2kthvdgxf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2wpaybouz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dxmxgdhm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2bgjwydhg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ciinbchw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rbfsxhhv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2bbpjebeq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2qusckigd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2dutswjam.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2zalhbarv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2spwfmldv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioqziapd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2srxixvxl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdfgmtkh.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hjhrxpko.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ujmtxzuo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ubwtgypt.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ynqaiaee.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tyujksfe.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2wvdlunho.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ilgumpyv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tksoxyuf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2hkxiykeq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2itnatliy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2htvlhhys.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2svhkgzjo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2yrxocbos.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2mzqlwlgw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2lrqftifb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2glfctifz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2hjhishdx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2unmpnigu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxxltogy.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2rbnyobjk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xsthofio.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ajvpedzz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2scpggdbf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2yhjazoxj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2krrwbgxk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gglibupv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mmaifcrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2syjmgtvd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2imrfyetb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwhnrjth.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mrvrmebk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gjncfgjl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hrupxcmc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2rsyvfewf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2tustipvh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2icxfbfkn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2xzjtrmol.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2bhrkdmgx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kxopdslc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2dxjboccd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lqriltmx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fqzyxezp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dxsyzund.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2eiyamvhb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qelukehc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pyntjrcz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2uoxohblf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zexzewyr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2skojttmj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2bbcisklm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2rfitohyy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2hnyozizn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2rcbrkflb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iayzsmsz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2eljavzqd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mubqhagh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uxyvbcla.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ozljwfux.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2spfvrsjk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2zgkmbyif.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xlsyntwg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hjtgbgqm.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2wksaqcqv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2glqhermv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2shgkwgfx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2qtvahubf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2eypgrbts.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2pbpdasdw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2iqhgugyk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bupkqjvs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2hcrpprxc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2udueayfh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2optofanc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2szeywdeu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2kwpphkzy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ukfyosuk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mnqgkmrg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tvzsessk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2tepgchvu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2uyvczafz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2btjedxko.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2qdilfpnx.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2jaxwzfci.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2abxlinao.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2tjxmkhrw.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2fltzrmcp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hrmcskhp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2pwqaxzuh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2xqputdjz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2sfvscfnf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jrdvjlrf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vxbbhbpn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2yzzdiyjd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2afrixjcg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ammpvnkv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2yuimdtct.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ioxmzqew.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2fmkolxuc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2sjmzhpbf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2qictcdyj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qgfzvnvf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2czhzqagi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bujkbcvi.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2jhvgndil.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2bkchfzvd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2drjfsfqi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qvtgqjjw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2aufsrifd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2cftiromk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2beauddqg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bydufcux.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2iqxibref.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2fafvycwl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tqqwixpf.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yydfjlqy.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2spyyrtlw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lnahihdl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2zvbfgblk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2hmpqwbgr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2wjyuarwo.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2rpsbwgus.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2yxnrlbym.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2mdvfnzru.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqnpkont.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2rqvaiitf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2encscerq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xjticudz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvvktyco.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xyhmkust.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ziqwpyuh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyjehztp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cettxzew.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gmokuayk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2fefpkteh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2inouqmnm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2echcesbx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2srifglfd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2doukmrio.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2auyetxza.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ccljynne.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2tsinotdz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2nhbpxwys.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fhjufvda.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zbkkuljv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2agaqyvyb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2mcetlpar.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yemsegns.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2pjplkdsl.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2itwsrfnd.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ofzoquiq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2qptdfkmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spbmeimq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2snbpsqll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irmsqojj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2mhkbhfxg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2dczoexcn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xknvykoy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qbwbgzva.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2yqcivrhe.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2tbpzlqij.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2rovuukyw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2dqqwdmcu.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2euyshimu.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vmwablfy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2yhfqhfss.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xnybgyqk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ncljfbpd.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2gfxwjrez.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2lajrpfbd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2cutnmdoy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2rldjvidj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2nussqtpq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2rqbhfctw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2dkggfkdd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mwbxieoc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2btahcltv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2lqaedkql.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2quxihifd.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2qpmxbnyn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2jjkkcvgh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2oveitddd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2xlsiustd.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qekvarqn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2akaawoif.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2oagnwdjc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2usltzwnu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2pwkoqxya.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ffcypoli.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vvbeatga.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2huticrov.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2rfqyyoff.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2onkaknip.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2eojlteuw.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2lsdawwof.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2cckzigew.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2cnuksatr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2hqhbkenm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2sqmvopyk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2wfrkwjax.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2zndhpxke.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2gcnobbkn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cqfpbfwg.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2scumwxbk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2kgjczeij.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2zthlmbum.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ltrzmsob.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2zfvukpgg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2weyoifvm.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2lupgmdan.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2sjaqlrij.html


<!-- 参考信息 -->