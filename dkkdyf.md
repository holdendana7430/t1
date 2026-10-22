代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pnykjqez.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2bunzdfvm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2wdidgmwa.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2bvpttvve.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2nehoucib.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2hxznysms.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ddyklbht.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2bwsavfpi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hkyggzoj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ifjzvrxc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2frnfmhfn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nsttktsg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2cteofngf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2hafsoohx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sakjrypa.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2nskjciex.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2apmvnnoi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2hokbtxfm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2bdcjdnfe.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2enmqpbxs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2rpgrknzb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2kltxbtij.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2fnfekojk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vrruobmf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2buleimjw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xldvtcib.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2uwvridqo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2kjxaqmov.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kjgccezk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ljlwumpj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2naziqokm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2wnheqdxg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ynlnipgf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ylmjkask.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2uwyvkcnc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2qzcodgdf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2mxugzzns.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lqjstews.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2bvszqkbx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hjisleuo.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2nhhiaedh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wvpmuitf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cdyxmmzr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ntsrusxq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2slgdllfr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zcrlsgbm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2semioplt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzaqmosx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2dksuvucy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wstpsnky.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2pwraflvz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mwibaspr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2mpjxksgn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lrtjbtjm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2uhrjgkxn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tyxeoddj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2fjrrpbnk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2kpcnehls.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2cboyntsn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ipzbdrmb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ijjumjkk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jaaiakwc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ulkhyxmh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2jlpbljed.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2snshhcgh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2wgonbsho.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2wgalbfvo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpicmsyi.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2qhdcmedt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2qrqjcpgn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2hbwmxdve.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nhmverwt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2qxvuilrk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2exkhvspa.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xrrsbwkc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vgfvilbe.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jpwffsib.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fgwuxrzq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2eldacelt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2zmgmfjwo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gpqgohlf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2lnygvrsb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2llobrtkn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2pybqttie.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2irlhgzpe.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2osbkttud.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qridcwsb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2yrqvgald.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2iakxiyoi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2aselwiom.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2aqurfjep.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2mvcfyqzd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpsvqrqk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2bjhkpjtu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kgfiqfbf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2tkfpougr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ustfbisc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2mcnabdbk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2fzuzfyia.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2forgkaiq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bdbtxuza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idzotrjw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jaobfdvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trrtzyja.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qzzryniy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hnyaxaja.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2mjftunwa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2lpcalpcv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2zglzelyh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2enykgorc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2mujyugor.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2fqrzudln.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2idvpdvel.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2cbfukzai.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fverlqdo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2omyyybos.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kbtfjmaq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2iloijols.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vhsklhtd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ovgqsnvl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2lwbpdylh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2yrsdbuub.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2uyfsirjl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2uwsurrpn.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2skqktsaf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ecqnffyv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2lgbbwgit.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wpblnbru.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bylyfxrx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfnejwha.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ufwjpflk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uscjueoo.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2bccwfxfu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2cpemgwas.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xhxtedpc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mahujipx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2oeiaiwrz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vundalvw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yhhywtki.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2iyloxxno.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gzudeyqw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2astswjsa.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2hcfafjfo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2huklbshm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2cvzarkvt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2kdleudac.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2wrefuruh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mpkrfoyj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qthfojul.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wbqwfdmu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2fhdffdla.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tvfpionx.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2bprfzbhm.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ovvfxuuv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ovfpzxas.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2cunhcznn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ckmyibqu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2dwxhycho.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lsvfzfnq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2mtaslkei.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yqrbgyae.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hulmfjce.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2gjpljzph.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2dzaclruf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xexmwssr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ixyjvlte.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wyahnjeo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wtueeoiv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2lqhgsemz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2usxtkobi.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2rrtiqmmi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2idzlbuee.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2scuiunwl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2najtxzon.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tjfhhcsb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2dknsiqtm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jawcesxw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2gutbbbpq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2edtkkbic.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2rmenymxx.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mhojnrhc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2tusybczm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2bbjswiar.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2iceolmfr.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wkogtzaj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mjtvgfmb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2yqatyymh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2znsohjle.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ifjtklnz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2erdzxwdi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wbosqcfm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2foopndbq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rqiwokew.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2yshilctt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2bdtsmtwh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzpebvqj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2iegtzwzp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2lormmqhu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ejubkcud.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2uawntjao.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yptzevkc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rmqhzins.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cfahateh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2dxnyxybr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2viqoobhg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zfesvdhw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zvessbxb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2byjupkuh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2wcmdggie.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bifaufpe.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zslngonj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2obfdtixj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pishpsns.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2moexwzxh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dyppgqvi.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2apjpugni.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tjptqwoa.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qohdjlwq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gahobdkn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2vhmqdmnu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2pgyojpoc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2cjserqzy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2svhkathu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2xaodvhgb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2fwcidcuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghfoztwr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2moysnlrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdwqhkmm.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2lxzdapsi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2njvlapaq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2hwvmxwjo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2digckfro.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nmunmwxa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2rclbczas.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2xllnskel.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2mkccxxjb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2gsubjcra.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2thdzjnsi.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2sffcnnfr.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2rovzthuv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2arzsidoc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2fufzwvxt.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2oaxxazjy.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2tyaqpuys.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ekwubxyl.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2dahfjerk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2exqdvoex.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2luqfoqab.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rfhvbcks.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2delqfqdq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rscubgvu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2pcsuwohu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kcevlylh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2bbeoyemh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2busfemul.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dzzqstzn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2eupxdqjj.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2zrnmvbkg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ijtmumvc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2mqozcgyl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ktdzfaeu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2avuwuigf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2adxkiivt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mxosaeii.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2meuyyxwy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2rjuybaom.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ijwnmysi.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2souxaquw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2wgkwndfq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2lkbgocfe.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2chiahxls.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ocuubvvt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2rnxhdyxh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2kwwuywpr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2pvhsytgw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2thbedhmb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2sqhnukay.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2vffnftgs.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2bqxctudt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2enfhuesp.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2yskebhtd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2mhvkmltm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2uemkaevw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2gcebxzdw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2vnysfcia.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2jhxgzwzs.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2clbjohoe.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vpkahbqq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zrndyyue.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2vfwxsngm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2mzlrgbdy.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2eiyfluqa.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2fbgnyulr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2rxmrqrpv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2fbzguvec.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2gtdrppnc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2sioyqlil.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2onrpvrfl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2wzbjopxm.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ioxfsajs.html


<!-- 参考信息 -->