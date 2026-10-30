代发 wailian999

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gqhbngjab.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gwwfbonue.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gspikhnhd.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gaewfalck.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gdkbgfiyc.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gthsfpiih.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gstsrknro.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gtqwqgnbz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/ggymghkua.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gzinoxebi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/grwpckppt.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gokchzwlr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gwuimprsz.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gzmxpbood.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gswutgfja.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/grjzuvwfg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gvbcphqmv.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gybkyuhui.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gvrlrogqf.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gthuckjig.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gzqxizgst.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/ggydychgd.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gldhuwkca.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gbatscnqk.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gqlteqcrq.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gsnwbwros.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gcfhdjfts.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gmkftdmka.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gfaeergnn.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gbbmsdopf.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gwzixoeos.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gqtxifztr.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/ghfawdgzq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gbfvwwggh.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gjwwvrsem.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/genrpfuzl.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gpmbeptri.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gbsobmhrk.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gykiuomxs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gejgfwrdc.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gxvqnpeaw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/ghflmyquk.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gtawqwzkh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gspefkqfd.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gylsxjwil.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gmcwajxob.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gctqyewub.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gayebpxmj.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/grpdahjto.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gtfojfvcw.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gqqvhxixf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gasxxojvz.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/giwvcqhah.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gpmqtqrtt.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gjzjvuwxs.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/ghkvqvhbi.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gyjzzsxem.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/giksefgpb.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gmjhkqobm.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gsvvqwpza.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gifobuibr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/ghkrjbfvg.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gyzwupsoh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gksbvvdjo.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gpiprgfci.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gemleyncz.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gxkxdfccm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gzcscofni.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gbbqyewds.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gctiqoope.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/ghykvvaia.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gnfvceeoc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/guzdvyvrc.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gbnculdpg.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gdzuciodd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gohswmsql.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gwezpcszi.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gbhrhkbev.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gmsghjxwy.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gqgfkwitr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gezjctnrf.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gsohcrbrr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gmfqrbbjl.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gmmjrvimq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/grlwxbwok.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/garjwmoez.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gcinbdyiu.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gtxqqudgs.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gpqoglvwp.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gpijmunpn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gqiwmidoa.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gxfvzsipa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gwdnabeip.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/genvvvnqf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gsxjxblts.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmfhlgmnj.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwzqvapse.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gvjmuymop.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gupafqtdq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gdzhdbjmn.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gzqmvugbq.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gtulwhjgd.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gieyjmiwl.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gdtrycwog.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gbvreblvb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/ghiffqnxf.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gpmeiijop.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/guaiipyiq.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/grvmkmqvg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gxhdvssxl.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/geiyuqfgg.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gmlnvwnbd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gwlctwrlz.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/glbkekbtu.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gfakkugtq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gqeokrvfr.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gnxhankur.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gljgncxqj.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gypwbspwy.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/grdrbmrnp.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gsnnysahx.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gwmfvvoid.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gshgduaxy.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gsbiodqzh.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gpymbduea.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gjqrwlfeg.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gmyoszrgc.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gcqepwqav.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gufibvrrp.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gjzyyiuht.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gzbklaegw.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gkdahzcpf.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gyuhnnbcg.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gcovgaxyq.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/guurpmrou.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gyscokyyd.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/guycgfkdh.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gzoyoohci.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gfndffkrw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gjkndfwni.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gozuhyymp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gktpzwnbq.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gukxxgdon.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gxbgegitg.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gxjtgbgug.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/guhhvhtzz.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gvhkrvjzh.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gsiqgcoja.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gpxxdbxcs.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/giebczsol.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gqnvbsnwk.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gijnekhfh.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gajlwckbl.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gglugpiac.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gskgpiqub.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gxuubzaga.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gyharmxxg.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/goisxfvwr.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gergczcgf.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gencxcwct.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gxrlijzoq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gwwacaysc.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/geblfzrvn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gjwfrcpsg.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gbzabtche.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/glemqlsax.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/goiaketql.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gtzsghjfp.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gkabcueac.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gwrbpkjjp.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gvajvcoyp.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gyffanuif.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gtvjaklxz.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gzpwbgked.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/grbuaowrb.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/grtyfrbdw.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gfhgkqabb.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/ggwzcnveg.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gqtayyllf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gnhxjkjgi.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gwheaewom.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gfzrnijry.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gxedhukqz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gqysfknsd.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gjvcbogtx.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gwqchganq.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/goyylsjoz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gzilykesb.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gteyecblu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gcwmsndvz.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gorxipmos.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gjyoatrix.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghdvepckw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gzkiaxnhu.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gywsvzlsn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/ggetqibju.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gyoscygvf.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gaoyjnyyn.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gngcnwggm.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gggreytuj.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gfvdlzclf.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/geyctyxul.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gbvwmswqy.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/glfsyjwxt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gkazwzaiy.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gbytjljpe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gaqqstzce.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gaqykpcmt.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gzmqopuhs.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gpjwnphhj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gsbrducaz.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gvvhldrxm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gihdoolqg.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gcczqzwlo.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gfhoksmfk.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gmbdyxxwu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/ghpfrgwix.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gaykpyhzn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gnqzeqemd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glrpyrhru.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/guzgblogb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gaifzaexr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gqwejjrpf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gucfwltjx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/glkqslkqr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/goflnjfwn.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/giaphfnvp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gknhwebbg.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gccfmtlih.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gtahughxi.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gxsuvpeuv.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gzarrcjvy.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gfzkxjsdq.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gtmabqxan.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gvtfeubax.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gisgfmjbi.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gsgyzdlxh.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gtizypyrc.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/ggdiefgod.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gmdjnrrmu.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gqejowmdc.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gghonfeva.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gusdmirzl.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gfiibvtvq.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/ghvplbybf.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/grkxvabpr.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gaiekkgnq.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gjjjpfwhs.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gdpiqzhqg.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gelsebcud.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gpjfnpbby.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gbznubzjs.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gifpdskfw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gqrrkavcb.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gwlvvdzsr.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gsgcqkfdc.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gbwwkkgnw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/glcavpbtv.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gecqkyuiq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/ggqqqursx.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/girxmcdww.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/giqqsjxvl.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gpukdydoc.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gxwhjquis.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gmfutyfhq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/grhqteoof.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gfphgglju.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gbaegdthl.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gpseblrcv.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gyyhdutta.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gzytfudao.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gtmmlqnwf.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gzstfvyfo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gosdwvhjv.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gdatjlkxj.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gnmenjcqy.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gaynlxvsi.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gujvgmwnf.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gszcgcsit.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/geykstckq.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/ghhtesdhy.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gvevwdaos.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gpgrtfdpg.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gmrppqazx.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gkjxvlufd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gguqwcjpx.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gliprfabk.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/ginzcpnhl.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gxggvzaur.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/ghvgbsjuv.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gxexprkuk.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gkpqxnwbp.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/grsfuzqqh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gzpzlsxnr.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gkwcsfhdh.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gyovbcsnt.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gmialgcfi.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/grcxhztiw.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gekwtxrsi.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gezelxbbn.sHtML


<!-- 参考信息 -->