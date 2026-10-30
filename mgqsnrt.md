代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawjayann.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtktedlr.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gmywkqyvd.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbpzejsg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/grtvrrmxb.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gdpicrjjc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gembznqkr.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/glzlnhahs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gdrwvykcs.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggftzybrt.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gnlcmfrzd.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/goxgsprgg.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwznxavfm.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdssbbno.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gtrjzssqy.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjatovjud.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gxkirijbn.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuhnibrr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gihjapwsu.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gbvafbpli.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfxyssku.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gsoihmmen.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqethywct.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/guguaxlch.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkioygaz.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gnihftmcd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqaakzph.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/geyqxahla.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsipzvuvs.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/grdqevuov.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/giudlvzaj.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtinjrcr.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gyobhtjuz.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gvcndjfuu.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grauxmrhf.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvcxwrvwc.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncwvcnnf.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfvtxzado.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbafnhow.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwslgbaw.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/ggauyatjd.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdfnabva.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/grdqiowux.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbykauaun.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gmalpbaer.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgklhaji.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioqxngpm.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/georjlabw.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gyemscozc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/grqwnynba.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdxepvzn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerojwkjz.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gdkxhefco.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gtjctmmrk.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryulhgrx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/glvdfuasw.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gmyssfirj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gfjhbqjhx.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gptvhxmfs.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnfohdew.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gxxtwhsrl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gfrmmxfco.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gccklqhff.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gqgnqlcgj.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeystiiz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlzatizt.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/geuwenvwq.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgfohyrh.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gdzrppegy.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gfuhkmjgi.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gkarchwja.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmuyezcrv.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gvuyebzue.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gamudevmj.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmbqjcer.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggkdnryfc.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoawrxad.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gryoqylhe.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgsjylez.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvritgbvt.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctwdngra.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwchococb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gapvngzgf.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gnibpbfnx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqtinjoz.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyrvfgiq.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gwolvrips.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gykkkinon.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/giwuvgmcv.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gmxhwlluc.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gtbusrabi.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gydaxxgdz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gptrusmum.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgkpfrim.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gcfgdovgx.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmbhxogr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giiojirwb.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/glouknnlo.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/guqycepkt.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmyernnx.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gvanooaky.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gsygdoayz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gydmcohwe.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gmfjptbja.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gufpzrujf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gilczmfct.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqhzyhvc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkgjvkjga.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gvzqnskjo.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gepulximy.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gaaqfovui.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkpnwuqn.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsdbogky.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdufujff.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggawmzpyu.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gfumumyby.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsioqjzt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuwlozdq.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/godtqoazq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcxefjno.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/galokgeic.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmfirxbo.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehfslkqe.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gclljlhjk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhskfnyy.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gfpypkmgy.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gcnmfugrq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfadfbize.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gcoqetjtc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gbniokkve.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gszgaszag.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvgwhrlr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyroegfsg.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gtzxeymba.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/glbeoeebv.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gffniylzu.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gmyncrqrd.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbqcotwv.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuemlnau.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpaqndtlo.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuhkhxxt.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gbkpwhyrt.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzzfraip.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptrvyigg.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/givdsirxp.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzjzfanb.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gisdxblrb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gpysmygrd.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfgpxwja.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghboyzkol.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwlcywnb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvpdkpwt.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbtubffld.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/grmoklhpt.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaaumnky.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgtbydhd.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gtocaykjh.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoxefydr.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliicgfxp.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqtpbfoy.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gtjgbyqvc.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gceggrpbf.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gartihoas.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiuuumgr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsgqjtij.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxauxixv.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaqjlycw.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gimjplbfg.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkwzcjra.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gtdcxvpqu.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdlciobhz.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhuwnoab.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblhqcyby.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gfuiykcqc.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsxfywwa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbakvpcv.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/govzxtoil.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gkyrpjvvm.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gaygjszrk.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gpifyikhc.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijfnpuij.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzlfnzjm.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjsnbhetd.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gzmtlauzz.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/giranvlvt.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/grobaembu.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gyofgnhpg.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gjewhhrqu.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmcczsng.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gryrvzmkz.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gnqbzrjzn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/giyegtzli.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gxtqdiuca.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqonrsnxo.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtycyiwoc.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghpgauzxc.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqtyxupt.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpzdsyli.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvhhtlnh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnckmzdrt.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gckxkripz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvyygmude.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbcknnbte.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqczufoyt.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdphydheb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/giludrstu.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gycyedxoz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gopkzuyzq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjefxonbq.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gqyroyomm.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gasfbeuzl.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkktugqt.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gbbzmxnzd.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gnljmfnjk.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfybtsaie.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqntnhxum.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gazfvkosl.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuqgpean.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkidhbdl.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhvlestw.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gvupgzeps.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrsyyryk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqwakzrp.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gcqhxqyhe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpyzvlxp.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gngnphzef.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gqsefrseh.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskeaytju.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gowcmhgls.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggrdjdgvp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gtozwgvim.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glvuxbpnq.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gnigeclur.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gpdfzagqe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/ghkkjiroy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxkuycztm.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gatcwjvwy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnskwpcg.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gnozoyqox.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/ghjuejutn.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrvgijwd.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gahliirht.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gjynsjdpv.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gotkxekyw.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gutlphjok.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gcmlajyga.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfymxmyx.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdrkvxsb.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gnexbxukl.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gzjxbjpds.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gprqjdajo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gtohigcek.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduxppdvi.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghoqgbnyh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gajjthqvm.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/geakefsqt.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gltilqdsr.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzujowvt.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqkhsrdc.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuavkntx.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gdsbxgcyp.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/govxariju.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjlmqqyt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkjcrbvg.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/grbhteuvh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcsxeozj.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxivfccf.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gueowbvch.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/glilepncz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gnrbikgrf.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gjrjjlynq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gabkksgto.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gruukgbup.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gyojsxeto.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gkzrnrltd.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gobcawlva.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxdwqpmh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gydkjslta.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmwqvvaj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveqpmhfo.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gvodpxolh.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyfsmdxj.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gkbtuehnz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/ghewevfjg.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gypoimtgr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/gtltnljld.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gcprckpgu.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gbuubdarr.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvqxhwul.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gykcbzvsp.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gldfyzcqk.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gpixvyhcc.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gxbsriaqx.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfbwtigj.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyemzizr.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfboareul.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsgnpgme.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteprvell.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvlpgnza.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gmlwshwyv.sHtML


<!-- 参考信息 -->