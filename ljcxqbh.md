代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdphuqej.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkqutlgl.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/grayhdkvj.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gujficxfy.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhxyiowi.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymubrksa.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gipvsukef.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkqadzgrp.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gamwvjhzu.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrbezwuv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjbjdhsk.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gnlpwzlgi.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhhsvska.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesgvzydm.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcqfyobu.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtropyjao.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/grptqdphy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgfhazdw.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruvznoxp.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gqxpchnns.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gcwjlvmze.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gmwgaywaj.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdetjmfc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkdxzewi.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzeagcwn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfabivcnb.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gxubxefen.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/guuowrham.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gokhfnkze.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gdlvvvijd.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/ggvhwyguy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkunwnpkx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpcyydik.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/grepieoyx.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gdgnshzys.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdlkvygu.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaztfyep.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuffwuii.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/ggxuozkuf.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gmgyboiit.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/goeiqugws.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/grdcutgsn.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgduiasv.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdpxtjtv.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/grdywcytu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gypdepokf.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/ginjemfhw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzipjgxs.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gkzyznmzr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdkpxkmd.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmkpevfd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gozrcfcxs.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gqyiaphuf.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpubskqqh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbeotbas.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnwdmmfz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqexkufwy.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/goaoydogf.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkibqooz.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gfwagfesk.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrpkmiwf.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/grubbaray.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gtmrfycup.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/grgxsnjpr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gwesdulua.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gailetcbg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gygouafbj.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gvmamzpfg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givjxlfdn.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufhlbkqf.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/geziwbcgq.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwcaiizd.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmroqpojl.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gssuhfega.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcihucco.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeuxugee.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdjmhmaf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkftvshq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxztprnp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gekahbrvp.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grighjveo.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gggriudvj.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmmqfojk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gttfvwlxz.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gllxysxvp.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/glsjcxetl.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gvarvimbi.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gahyqdipl.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxljtqba.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdfnaaqn.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gxzykykxp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxprbeay.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsmlivjw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuhbnkmp.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gmenzpdyf.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/geodvasun.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehggrzhe.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gakzcwrgn.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gcnblowbk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gsypaepse.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsuzbbrp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/grddlwfpp.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gouzmkrsw.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gygbijxpr.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gcrhshkbx.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/goezkwhkl.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwkseopr.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyzneujj.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gytywsecb.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcblvhqov.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjbqiyet.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gsbeooako.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmisuakp.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gsdjshnze.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gjlgxgjmo.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmqpopbi.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsglxeazz.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/glzzsvxtv.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gzaebqvzh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxmsxvpj.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gubgapyny.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gmqyczkhc.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcddmdom.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gyhjztkyy.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqdyegscz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgkpslko.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpnkubtf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsqguzws.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjihrtvl.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gmupiowgw.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehfeukwz.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gygcgawhk.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gnlgfxtil.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqheewlc.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gyqcbcqsh.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gexjbhbuu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrvvhsar.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbiethof.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdserjitf.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gcsbsmsrc.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gfkfpapbn.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gylvaktsi.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhwqhjgk.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gckavwpnt.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsspmfgj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gasjhdsqz.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/glzvoujzq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvljftdx.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gmculrfds.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhqddfsn.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gipxebekx.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gcdnjespm.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gwcfgxdtd.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbahofbht.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gdtrykrka.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gtrwsczaj.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqnrlbjk.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbwtrwbx.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/grgcbjioq.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gocjsdqto.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gpozjepjt.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyywfhcrg.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gowcmfeno.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegdhvvje.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gplpzmgha.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gwmndocwo.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gobtnwjga.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxvrlvfit.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gffikfpfv.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwtnpgyh.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gwjgcpquc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqhtfhgu.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gofxhhltf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gndidzzbw.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gzczvmyjq.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggktkalsj.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmhtdtjlg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvrryucsx.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/goepeoqly.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgvzvsjz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzshnaed.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gysbybthl.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbeymmpf.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/giomtpfra.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gklfoluqx.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkaqbcga.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gcphddahe.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gpexdijxe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gsrtgndwe.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gsprhdxwk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/giqymuxnv.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcgwrmdq.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gyntdwkqk.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvfiwuan.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gacvojedf.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gildejsoz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gvswrhbyw.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbyeixee.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gzipqbubi.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlgcknyq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gexigswtn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtemauar.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpswlqhys.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gplpdjhqt.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzxzewxj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gyqpuaxef.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgvkdnir.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnkoxyexr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqtmndyb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gndninpas.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gyozreodu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gioiyrpqg.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gqpvurvth.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gakakmmci.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzpzfkyi.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gtgptoowt.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvoayciw.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjwiquvp.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gcxognfax.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghokrhrpd.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gbfwfxeqk.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gdhlqirrw.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/glnjjumnl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzechyeh.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gnygkgasc.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gjzzosfwl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgvcddga.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrhwqqkv.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrydaewq.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gdmvrxmms.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gdihfycyf.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpmnnyaq.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/ggzpmghqp.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gblaxibjn.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexrwjauu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcilydlm.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gnwvxxcse.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnlnbqgs.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gwasyxsia.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtehdowyb.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdeyaoaq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzgefppt.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gpldomqgo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gtnnzorje.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gcctkmxql.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/goylhazrk.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gbzyjugdv.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gacqdetko.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyyqpamjv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrcxepnp.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/grxezpldp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gtbqqnram.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdweedms.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gpmogtguq.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gukqazecl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcloijlp.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gifqkvfmw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gzerpbukd.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhbjvarl.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/ghaphkdwu.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkansfavu.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gyyditgbk.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gmrkhumzq.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gczucguby.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gagfkxthv.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/geciwbzms.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbdmgmzl.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmpoybmt.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gyeofwxwl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrsofjfv.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznqcpzmx.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/ggnsyvcwc.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/giiljoxjc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/grrumzgza.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/glxlstvgy.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/germjscak.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrwvwohx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gehrjmecp.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyeyaoaz.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gdtiirjvs.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/galtlrbag.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluhiqppc.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gaxayljrx.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gdtgvhypt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrvvryhe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gwavcpomq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvhoxxbb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvytwalwt.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnexbpika.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gsddlpauf.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuuzqpss.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/galgfzjoh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gacclvths.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gykybqvpn.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyqtdgnf.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gncrqauco.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbenclnnd.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gpzgbjkww.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gbhmrbnmt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsoarmgq.sHtML


<!-- 参考信息 -->