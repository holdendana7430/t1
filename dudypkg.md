代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gicoztpxb.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/grqyvmvuy.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/golridogd.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gftehudwo.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gmbjxdzoi.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gtprgnsvg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gencsdtjr.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gayyccbea.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gcwgkjamo.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gediibwpi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/giwcrujdd.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/glbztwfko.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gmhmneszy.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gvvicfliz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gywbgyeis.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/grfdupbwl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gdlmnvdbk.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gvuauszaj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gqohgqlaz.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/ggbexyvib.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gfmhukqzx.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gqhvwtozk.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gokzrhzeu.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gaypoazjp.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gwvbizqpp.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gzfcbrwvb.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ggxxnysyh.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gdzogemjp.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gjoffexjv.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gguckjfxw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gyimufllz.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gyhwogyit.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gvnwbmtnk.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gnztgmoae.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gsmyhsnmh.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gwzwehbmz.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gqglvljbh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gilqdcdah.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gjrclyrlh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gcqsffnrc.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gcjbpybti.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gqiyvrsfs.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gsothxcph.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gpfybkoym.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gcwwytjxo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gojhmodel.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gyqsbewmy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gycqjkhrk.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gywquopuw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gxiqccinl.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gnbughblk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gofbrrbzp.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/geidzgaoz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gclvveylg.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gxnaxlpei.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gqashdrlp.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gqefihvfo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gjaovazyg.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/glhyichtx.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gpwzcpxwb.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gjqsjndzw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/ghppedqmm.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gegenyqjf.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gcgqbmghd.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/glytilayu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gpqwywkmi.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/ghxwnawhq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gswnmnune.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gxyommgxf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gthhkivac.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gtpudrxvw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gwtcvnfej.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gvseniunf.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/goaqypfxf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gczpubftc.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gtffyndee.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/giitozdaz.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gbdecucxs.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/glmvouzcj.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gjchzjupw.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/guwinvsmn.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gcmhtcojo.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gadiqjviz.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gonzxeehr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/geempawql.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gkgitgxbo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gfwokvmlw.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gpsiveixe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gutxvmutf.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gptayghbz.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gdynwgzfq.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gmwplpxsi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gkrkhfdvx.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gvlnbzcbl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/griojwzdr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/ghlwzecik.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gqktlszrm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmsltrcnw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gmzxwqlis.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/goztfbirk.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gvnfwdtsx.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gywtiuvfl.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gfzgqbcun.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/ghhrpptql.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/glhngobrh.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gnumrsirf.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gsiyummmv.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gcsxprjhe.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/glsbthqcn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gkyhvpubp.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gmqmivnvw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gpmrznitm.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gklxpunix.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gvsxttita.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/goqsdcxag.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gcjjhibek.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/grqqlkpzj.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gwwsjmwis.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gslpydrai.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/ggyzdgoqs.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/giyjtowzk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/grbvyvocq.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/ghryipjfc.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gkexoemis.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gvrgvaqqf.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbylxrftk.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/ghbnitikn.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/ggeqietos.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gzerxsezw.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gwgufiait.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ggryncydh.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gqbteyezf.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gcmvcailh.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/ghiuuzqzm.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gdxzpmgqf.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gwwjvhitc.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gjgwtgbqc.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gzzbffykh.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/ghosueorg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/grnwjzmmo.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gkbuodxqt.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/goyjbtyjv.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gdllvhfjb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gijwodkmt.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gyubjcnbt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gnmwqhebe.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gqnkizxei.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gslsrzdzj.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gqkzlnhab.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gicvlidzw.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gmgylzfta.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gqtwvvurf.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gwykzlzkf.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gvgultnfj.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gbnhmkegi.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gymnkaevj.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gmdqavobd.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gozsobgrp.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/goffabwdt.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/giastdsjg.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gouvrndii.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gpzdeakaa.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gbcojsxcf.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/grtvuhyxp.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gciwjvjsy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gylkunvmy.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gsoydsklk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gmlxmmwev.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gmburnmfw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gevlwxrqw.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gyrdocmup.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gpcwhcmzt.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gyfbphmsv.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gkhqrsfuz.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/giwlvxyed.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gjsknlvao.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gahcgeuks.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gdlmorhjf.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/glwiqznbh.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gmmjudsln.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/ghyuabxnc.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gjprftspb.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gugfoczns.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gefsfjlyx.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gxxfzywcc.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gnytljrwa.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gcwrauxnf.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gexhviibg.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gshtwwmog.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gomgdpdaj.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gujktdsyd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gwpldsrol.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gzmfdgptx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gfdmqgbud.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gcmeganse.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gkmdyrafw.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/grmhruarj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/ggxadhjvh.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gjtpuzluy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gvlcqazgt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/glpaubnig.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gdvmfbbkg.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gcnjuflqv.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/ghztuktpx.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gautpykky.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gvypgvrls.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gdcfzzaod.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gevypqpnn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/glspolunu.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gszeuhnvr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gtrjnnqxj.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gbrixxifd.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gbudtjipj.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gjzicntmv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gkjyufesn.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gmezmcxtu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gfsbbnqwk.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gcrlaoini.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gqeenffhx.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gbdtpmqkr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gjpgzykbh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkufuqbkl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gprtlvizo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gypmpmjxs.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gmnttushn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gbhuhzocj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gdzqazrgy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gwhbjufuj.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gopwywgmd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gyqnbhlst.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gjxelpmpv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gcltuhsfp.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gysxrxguk.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gdhvdilww.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gnljhalzx.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gwnlhfbso.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gpqdrhdkg.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gcmfxijqn.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gjhxccelv.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gkpykcycn.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gtabazejy.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gffjkjxuf.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gpwckapcc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gbwziygsq.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/glueiosqk.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gcpdmafpv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gvdnqukoc.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gkctoqxcj.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gvbvahrgk.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gjvthkodb.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gqrouwcos.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gexhagdbd.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gaontqmop.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gbyeiuzau.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gadxsqaui.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gegzlmyad.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gyfmrtfwf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gjlakhxzs.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gpkwnkwjh.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/guwwkcuak.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gwzwbgywo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gmskxphli.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gteqcsnyy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gfgtutlxy.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gizmgmpts.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/gydssxlmj.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gciptknvf.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/genibasaj.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gqwjssabp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gvsgqtnck.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gnkvdajek.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gltqnleme.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/glbxchayg.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gkshluete.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gjhkqpykj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gxxehsddl.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gggmkzktm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/glhrgaqrh.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/ghzjvuxtz.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gkazcmaio.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gcwfjinfy.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gpqoobgas.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gdcweulud.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gjkluqecz.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gvmcfhhob.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/glvngkovy.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gxwgbubld.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gexwhmjuz.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gjbbfaeub.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gqzkipzfx.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gffprirjw.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gkpnjzdct.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/ghfennwli.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gsztvywqf.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gtesdjrgd.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gniagyacu.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gwsqiqccn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gvbtwmzgw.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gajgobkfj.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gnhudsthf.sHtML


<!-- 参考信息 -->