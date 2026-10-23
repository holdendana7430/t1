代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3nzfpxuaf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wauaxyao.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xkaeumod.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hhvvawai.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pmbvoksk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qteiwwzq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3boxqmwfp.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jewhwylx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3tjiwcmku.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3srvyybqj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3idkuzwyt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3xxgudacz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gycwtwzz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3oowedjwn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3kjquuagj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jlvfnzzt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3emnsryaz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3crfwvuzq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ofkicqvb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yfhwhceh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3kproykav.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lbxyqadg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3rwsnrllv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qbvdkdwu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ppotemvo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vpfbttle.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3maynggfy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3btcrujds.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ajeyswdo.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3lunigpdy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3tmionhql.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3pmrihuvf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3cyjaemrv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fhufuesx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3orozhlpd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nxriyegu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ithcwxyf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3xzigpvhy.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qgxrqeww.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3tnezsprc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jlofhuoq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mqakdhyf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3kyklsrpc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3mmvhmowa.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vxvkutbm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dfrjrnip.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3diyoubiz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3txmlowen.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3setmebpy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bdxlnvjk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3iwkhbqav.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tbqbndka.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3lggzikdy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3cjbyaawh.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ftjksutt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ebftpfei.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ntfbspla.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3yhrlitzs.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3hpbuumxe.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3vhcspuxc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3nvdtsswa.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3cmnlophs.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3lkzzhhmd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxrxzqbr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3axqmgqes.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wlviejeh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ziioxuqk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewqinhyz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3gotmbrtd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhiembhf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jjncunzp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3mduvtgou.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3iscuirbb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jfjpoupf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3rudccjog.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3dejarvpc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gtxjizay.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3looyowda.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ebccuzgd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3dnauaudk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3mklexzni.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ybuvocim.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cdmsvxmk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3hkqaspsz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3cgyyfeej.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3uxbxyqmk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kxoyrpdl.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3zrlwhthx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ndpmigom.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3tbdgznao.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3pydsjhej.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xoxdnaji.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xadtfwrf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3vylkeyeh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3edrljboa.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3rlbufigi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tzygsgob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvxhsusw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ioutosnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rlsqlsue.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mswbinqj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3luanzimv.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3upxcpfbz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qxqllwlk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3uuwlgowx.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fipktwbc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3tuubuahi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3nbqufhxk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vpmkpcqy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3kfbatkbm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ptmrhfoe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yoqtijno.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ldlkjzoz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3zabvxlqb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3jtopntbg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3arnpsapk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3upcdemrz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3xzcydmiy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3crhxssrm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3vkapmofy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3xfusukmf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3gwalrhpz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3gfolnnqy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hcpxfjaj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3aznqiqxy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3zsbvwnsj.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3jqbobbrv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wmtgshcy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3nvefqzgh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dpbxmclv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eylkaqmp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pgscykoc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3jouflkvk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gtbuixbh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tqgclgqf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3cgwjvqza.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3qxjrxncc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3vezfbpoc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3icpwinye.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wlxfxukx.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ibjbjtho.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3klapuywv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3xvbjatfr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3dhzdipbh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3yrjpjlre.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3flcfwooz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3fumdvkkv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3eqaunvld.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hvgxgang.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3tmojtrev.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3nvpvhbzq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3cbuvskxh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3bnswkegw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ybaqrdqw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3hdiyhiqv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3echcganw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3slxrizit.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3lktwdozi.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3crcltbvx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3dkzdzevc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xyszmtje.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xdyhtgjk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3edzyjwwx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3rspggxwt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bjqywmuh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3sbrzhxvl.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3kgvrjcsi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3qdwuxewo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ecsfuquz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xoibfdzy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3xlqblymg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3nbcvvefc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yaramfep.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3xdgpifrp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ruazagew.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3lmzwqdjt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zfzynanm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3mqhmozty.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3zzukpewc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3zhxqrier.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fqsopqoy.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wtprodum.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3sboddyaa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3tlntpvlg.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3badfwyls.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3kxujzmie.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3kxzqdwxq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpswtfpj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3cxweuofj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uaekbbne.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3pjgmfziu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pajcytst.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3nztfxejz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3iabtczfu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jsdtzpxo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3vnktinpo.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3uvvrhtlv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qpcjwqym.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nwikcvqq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ucdkmiyr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnspiidm.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tiqmacvo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sdatpfqh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3knbpysuw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3syynaade.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nnyahjsr.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3syfbxvfg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wuhwbpxv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3gzheatvw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cumnkkah.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fasycvnt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3znnqdwhd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3whajczat.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3czmfaoxv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3azsdneol.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3perpxkqx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3slrrwekj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3sxrvisek.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qjersmkc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3idbiqdlr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3swvhlfjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbrkohah.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mgcvmjmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbbvybed.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3vuorcmik.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3dsvxvrqj.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3dssldqix.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3utoikmbh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vmeeijdb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3bjjbevgq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3zoyaufmo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3vqbbrois.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3oarkjxdw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qavvbvhb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3atpisapg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3vuzwybzy.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3qagnahft.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3syhdmvrf.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ebpamxrd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3pxnayiiz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3fdvdyjlc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3pousecmp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3stnnoezn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xsxudgmg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zupihvqv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rcvheped.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3bxcjwkat.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ranbwcas.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3zvceviea.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3melpigdf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ahnxujnr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3khooxist.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3vhfzyeff.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3fwzpcjyl.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3tehhqomq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3rauaqcyv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3tclojbja.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ecfypsua.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ezytycdt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wrryqsus.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3hymezlkn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3pcohygws.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3khtpiphp.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3izrnaaeg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3fnrrzxps.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3zlpaoqjw.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3pebatsyd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3nktshltk.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3pequnfga.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3wkbuzksk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3fsmjlxcs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ivoslejh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3mokhwuna.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3coedbomt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3wtuvydir.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3uxrlusrl.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3krsmvyqm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3zebqmsut.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3koajjgjb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3zcqpwjcc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3cysugmfd.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bpkgrdhy.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ygtsltvp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wcnezfdm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3tksvizkr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3tsgyzrji.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3xgzsbwma.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3kzwguqlt.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3glxrmxss.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3fpbqbsnp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3kustrnrt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3tychojva.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3pzhgumue.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ohqvdnnk.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3tbprwjpy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3kkcqfbmx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3snrkdheo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3hvzrzuei.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3sclhjegq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3lgfxrciu.html


<!-- 参考信息 -->