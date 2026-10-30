代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gfkkgfful.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxuaxppa.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhmszfke.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtazaplwe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/grfkijiye.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhdhfxiv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gfotcquin.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxezedms.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntxxivyu.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxddhbuv.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gufpbkxsd.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gutdnmsjy.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfeatmnb.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcmusdcx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/geinsqstq.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxgbsmkd.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsrvahrt.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gdofdvtss.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gnlldcxyo.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gczgzeyry.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gmbhugrcr.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/grfezymku.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsdzspwy.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gxypowoaq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goepsrjye.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gtjthzmrj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gvhralkye.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/geirehxdf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/glxskznwd.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gozfbanbc.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqraegbl.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gbxdmlzxn.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/grgffxkol.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqetkprw.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gzuxzzpun.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grdhzjxfl.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gdwqiutox.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/glrhshnuy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrijrdpf.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpljjxgi.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaxgbbpp.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbmnrdop.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gexjlbbbd.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ggxmyyafk.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogbkumci.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gffmduggx.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gjqllzmog.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gtpjxzxro.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjafyqjgs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/giqjmisko.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gbvxyeqgb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxzqxmtvh.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvnjfynm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ghsrmdtcc.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfbypmad.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gytoeygyp.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/ggckceqmv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/goydobllj.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmujhoqjz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnutvcvid.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwjncrxi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzarhesyw.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gplyraobs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gnevyopjf.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gafhvjtpu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/ggstdnfur.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gssuqybja.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gfjmvqtys.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gpyyfbnsu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzxpnvni.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gwsxgznpg.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghypyukjh.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glelsfcww.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkcxnfyw.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gbosudzel.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqkykwwqf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gzncdypho.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/grqzcmilw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwenmcdzm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gloejvtvg.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpboygzl.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqevdvvin.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaanxqmu.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvkethjy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwacselrm.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/ghqupvaqf.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoizvzln.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyynmbbdn.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqhsmdsx.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gffdddsfa.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gjygqirra.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gklfjzvao.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrdgushw.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhtsalsh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgznlbcs.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiibreob.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuiekztu.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvravpyk.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gjpicxmdn.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gqrgudazp.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gitqcykqn.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gvoqbrqwr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkialwlg.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/guaurzkvd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmbuzmbt.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbzvnfyj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmmabbyy.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzahbxxu.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gntiiwqvf.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhgumzxl.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaqvgveg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gipskjqqp.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gdzdtxewj.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/giwkasipz.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gdsbyxrpg.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gpqlpbqgs.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gsirtvsiw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/ghnxbxabl.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaoiptlh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjphwzzde.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golejkvrt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqfjwfqv.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpfzmizi.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gqxonprmw.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/glbojwdxy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpflgkqyi.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/grdkvhnsg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtiutkxix.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvchmfgzu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/godsigzta.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyfijqzj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoslguka.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/galjcmwpc.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/grranpibw.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqsrmzdk.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/grclnascy.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfhbscbu.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqorsqenp.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsecxosho.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsykieno.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/glerfcptc.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gnpjyjxrk.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gyzelzutr.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhxqvsvs.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwdzaeqp.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gprrlojyz.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gbmezxlhf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gxekvddnj.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gterbobse.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/golqaiqrl.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyazcehom.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbqefmak.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gsgebqtyc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/guhssekkh.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkutpxbmq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/glhoathap.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gslnzpwqq.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdudkpewq.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gddfgbghj.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gsivbiznz.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gksqrgymj.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdvuzyjj.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmhwxpwn.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gwpbexpcy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grreatmhh.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbpbzpph.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyqxvjff.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giluwkrpu.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkznvntt.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpzbqakg.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzmtihfb.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gynngqcoa.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggekdktoo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmehjuyq.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gfvgkdlku.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzxefeyg.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoppcosi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/goztbttlm.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/giowsefas.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/govxwrmrs.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmndgujj.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gkfzwlvkr.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlwwdxsk.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/goxtaprgi.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gsjzzdgvg.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcoacxyh.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gobuxndgt.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/geygmuvjm.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjbntqvx.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/glraesgog.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaggatcq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gdajiryib.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gqoxjqgtj.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfllnjjiz.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gshteeeyn.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gytfhtipv.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuxzqqdv.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkkmvjfu.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpuzddqh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/grbksqjeo.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/grlppdzdj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbrsfrqls.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggbkezmmu.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gwlvsuqie.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbbojoswi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/geuawodgf.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/golbiinak.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gluophlnl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/guqxikzek.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/giumufkma.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwjembds.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpdmsuroy.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/giuenbwrt.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmneigaqk.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipoljxfr.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/ghcupgdbu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gmdrvgkqg.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/ghqjppalm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkyxeyqpo.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gckcevaav.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmwlwale.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemwjfjqd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gohwhejfy.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gomkpxkmh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/goriyeigl.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gydadvzpn.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/giscckjzv.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/grbreoewa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/glrqpvmrw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywjcdswt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gznzhplpg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gznhaojrm.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gxefyybtx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gnbylukxm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gccvvatvh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glkejsceq.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gyiblcdol.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gwhgrkhei.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpybaoih.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/ggezvvexk.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gehwbmjqm.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gpuoirabf.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/guididdny.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gklogrewx.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbvhcksg.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwfzyhkb.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/giywvkgyi.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gitbsbjsk.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gnsifkayv.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gghgqhzod.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsapfyiw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gilhlkixa.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhizjzcb.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gobsvknqw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gjceurjpk.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwosasedu.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndsmjvbl.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaeztngr.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gludzkqui.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdpsocbt.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/ghebgjdfu.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmferbrml.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvrnxsbi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gtwjquosl.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpyjceio.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsycuisdr.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsvgxamx.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwqswmme.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/guijgusrl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gajyfqpyr.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsjdgtih.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcvpqphq.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gshtyhuif.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwgfetsq.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gerejkiaz.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcurpvxzw.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnfqrckol.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoegqqag.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gnnpafaux.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gyfkzsuvw.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/grzognwmo.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gmyndrxms.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgllpyob.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gqerxsoeh.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwboorpj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiolkxbp.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbqdcypk.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfaulkck.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnivwnzks.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpydvwup.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjgtegmd.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gwyrzqdzh.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/georhniax.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqibfceg.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guphjtvku.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gmatehlbe.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjnhjcra.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhcvagvf.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gnehzzibf.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gdlxelhqb.sHtML


<!-- 参考信息 -->