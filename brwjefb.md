代发 wailian999

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gsrdveoag.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gzzkvydgo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gfqsirktj.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gkusjrxae.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/grepchscu.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gggltsvvm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gtqnokcxb.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gbjbvzhot.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/ggsudvjsx.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gvodsdblq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/guydvqcpe.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gwdmvtgrp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gvxsembzp.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/ggzssvles.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gxozrrbzy.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gxvnrwpmn.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gtccavzlp.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gtpndsbdf.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gtvhlmcog.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gapecupzg.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gtzjuvjhd.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gfnjffrzc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gdawvejwh.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/guhktrzpc.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gyuumytld.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gtejkafpc.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gcinlasfz.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gpxylkpxh.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gdyprgvxr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gbjoakkid.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gvcoyneij.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gvpzygqas.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gypyshimd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gsgfwcdtr.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gqflajnxx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gexahjmhq.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/grnkbdqng.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gtraaizmc.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gubqoyafr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gskkkzwur.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gvzgsccwa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gxnhnkpmd.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gldesodfi.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gepsvebng.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/ggqnbmofx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gykhjcnub.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gehildjfp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gnqvtvefm.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gddmlmnue.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gthezfgir.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gwzyfdxcp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gimslfqql.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gaxsbzarv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/getkqrtds.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gpbyezknz.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/grdtrfita.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gtxmacgex.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/grdvbygfp.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gootadbbr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gloqolxeu.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/ggrcyggbh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gjfxsypur.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/giommijmq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/goxxfproc.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/grmnpxssb.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/ggunkdliz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gkbaxsudb.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gnpipbnfj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gruytvfxz.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/ghvwtvzno.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gvdhabqnq.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gybebbuid.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gbqzcvgfg.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gplwjjulf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gztifcexm.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gmlsbyfvx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gpxkszqcn.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gimqcxjyl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/grjnwqpwj.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gcngyumyz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gnwoeflig.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gxoiplpds.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gtgfmofrw.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gjawupidr.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gyrohbqoc.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gqufeeaba.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gjhqcjbqy.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gpwhlpwoz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gqqbhhdwz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvpavlcul.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/glycfkced.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdoayyagb.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gvikasmer.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gxnzfnaef.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gfekyqhht.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gdwezpgip.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gvzqwaprw.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gfsmfqxor.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gouinsxja.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gjmoplofn.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gengfptmk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gcnknxyld.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gkketdvrh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gewnqjprg.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gnegyxsfb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/glbrciekr.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gegutlqqz.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gzddcusrn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gbsgfbuzn.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/girxdncgu.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gkvmduswd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gdentyvso.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gztvcdaeb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gojbbkjuq.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/ghrowflir.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/ggeexauvi.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/guinqtizv.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/ghfmbkwuh.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gkdvfqbpn.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gadpjeird.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gzdmvnscf.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gloerlukr.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gfxgnfgfk.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gzovitizc.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gfxantfli.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gyhzffslm.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gtqgbmypt.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/ghkdmuxzn.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gyxpkfpps.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/givrahcqi.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gebjcjtja.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gtkjerxxj.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gwjvxqufb.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gcqsvzdnb.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gfnxmwjyd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gravbbcwu.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gymdotomp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gslgvhbvi.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gucjbhfao.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gocgmsxxv.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gpuyaxruc.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gkivqifjq.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/grojmkepu.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/glgqloyos.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gtjpttsvm.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/ghppjopok.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gbmrkspjd.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/giqeoeixd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gkjxbqqwc.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gjbfeexay.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/ghsfuosvo.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gwnokshtu.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gbxizwsjd.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gwfswlakc.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/ghmhtjdbe.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gejjfwtpk.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gzinzhecv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gfoqeezuv.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gpzzzycvk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gwfholzhl.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gaxsiodns.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gmbeesamo.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gnntcjmtb.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gcqoydstd.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/goqhvopkc.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gffppivck.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/glfmbuesz.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gillegnoe.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gnoqvdtlt.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gvfizhuin.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gtuewrbjt.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gffnbsysk.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gucnkywzq.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/ganjflibs.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/govbwshee.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gdsdxbpbw.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gtgcglkap.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gzfwhwchs.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gzoxrvlxz.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gjwjkzulq.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/geeitvfmq.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/grupuiizi.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/ggtyljfqj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gcsrdmusd.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/goqbudboq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gkbgmjmfp.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/ghpvcjssz.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gltvfahum.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/ghplsfjtj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/glcglycuu.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gaceqydmg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/ghhpwluil.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gtfnlicff.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gwexujblz.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/glnvriabq.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gvjmzaxer.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/ghpoogxax.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gktbqnvrl.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/glcpiyrvi.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gzaiszkaa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gfwzbozsd.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gnqqrutey.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gofndgqsw.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/ggesjudpn.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/ggmiwderz.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gnnyoxtfk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gtqkpytsy.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gkfcsjllj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gpnndilxh.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gkpylsyqc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gtermpnad.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gldurhcbe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gwvnbleoc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkxmweklf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/ggmelabpl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gogzjggdt.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gomfugcyg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/glrtgwbbs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/glioyjznm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/giqgpvsud.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gnypeofgz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/ggjqyzwag.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gqmkqdfab.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gxwwdobuz.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gaotvyisn.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/guexwfvqd.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gnzgoeunk.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gimnioczv.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gyosgmuks.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gdedhwkpr.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/glwohmagd.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gcfagnmht.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gekkfoype.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gzwjiklwy.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gszqnlnyd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gpczggpxo.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gatynhnsz.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gpvhvjphm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/ginkxlpbg.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/ghrisfqvx.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gaucbynne.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gcglxdrrk.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/ghpavifgh.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gwfejgrqm.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gxsbgfdih.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/govkmebuo.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gdlszhqcn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gevgpyokp.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gylsgsjde.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/guvcgobft.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gmvqlfvdx.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gdxukycld.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gfdrbvuuo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gpyuapiry.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/ghhonkbcr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/goiesoawo.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gkuvjucwe.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gmuthgqfk.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gsiklfpnm.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/ggxbufotb.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gcgjzptlc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gqbjdgjzp.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gafrfnqib.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gzrxckwmy.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gdlcoqjup.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gzmxfxniv.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gmcfqptzz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gjirsmqsj.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/guwjwtfdm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gdtijteuu.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/glmmtdjbm.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/ggrycbhgq.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gyzotdrac.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gdrmrlbhi.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gtldzmcmh.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gsnggsjhi.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gssjgesmm.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gzjvcgtpm.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/ghilukhdd.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/golzjiobp.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gbcryutwx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gjparmhfp.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gaggeovts.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gdbjhjftk.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gmlppywjt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gjyiczopw.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gjvvnjftc.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gugxrimyq.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gebfhtgdz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gsijvgxwn.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gieyodtyh.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gqgirfaws.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/geynguksu.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/grvrvcuuz.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gzeewuziz.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/ghbviffae.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gginygrjn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gcnhjguzq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/ghvodrqnj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gthrqbksu.sHtML


<!-- 参考信息 -->