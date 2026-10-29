代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gvnmgwyfr.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gdciedgjn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/govsajbhh.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gdmfdcard.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gslgqasjw.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gtxqxicuu.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gnqbjasad.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gwweokxic.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gpxriggrp.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gmrmumwrx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gjsrendax.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gwslxtukq.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gcqgidgif.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gvxpsqpti.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gaadlydhv.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gcyprcuco.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gbnmfytlf.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/grgtohqgp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gauskftez.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/giosuxzug.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/ghtwdifmg.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gjqjzuydv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gouwvpsqz.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/grnkloidc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gontdrocu.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gehgsoomw.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/ghmxbkdlr.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gycbcbhrq.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gqhxzqaqj.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gkazcqjmg.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/ghqsncrmh.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/ghsujxyiy.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gcelupfct.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gwawnmeqw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gpqzuihzu.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/glgunchim.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gkizkxlqn.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gembnhnmj.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/ghbgwnhiy.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gfvtjkybb.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/geuqqvxke.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfvrxweqg.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gwomaaxie.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gydyvdcah.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gywzijpty.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghszxeyys.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gerqltgoz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/ghtquzohe.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gqnxsgind.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gqjlaudas.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gtqikevhr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gvhicyxey.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gmafkcxpz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gwabmwcfv.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gqsfybyur.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/ghrprtost.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gqqvfasyl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/glyxswdub.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/ggnohxrzl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvoqekosd.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gnkrcysda.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/guxlvjlwt.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gwmdtjfhj.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gbsgjgpyh.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gahkxnrld.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gtxcuwktv.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gvplcggin.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gjjqvrmpv.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gfmzwzrkd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/grgpiiyka.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gtmeowoph.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gjyalsdpg.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/ghuroiybm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gxiildlrj.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gvoporlkg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gtcwgqyly.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gmvbcfbvo.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gmrywsuew.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/ghkhualqj.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gkakkibdb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gqvrrdplv.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/ggimrhnfg.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gbjucecjd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gvplamijc.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gnspkpdmm.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gxinxxopa.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gqubcapvb.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gleleskvd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gcsxgvqpi.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/ggxpmmzyq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gjafczuuv.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gptskzbyz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gsgtyivia.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gzumiiwlj.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gouhzybrb.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gyqsnafmd.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/girfikkje.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gmsgfjsru.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gkpstatbc.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gofkbeifi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gumvleteu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glmsmuqee.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gqmimsvqp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyjragclv.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/glondnevf.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gzqoazned.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/grplndrgr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gpasffsvf.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/grjexuesd.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/glxwkbbmc.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gnqjhjdoj.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/guugmhmfo.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gglvtwziz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gqikpkuko.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/geqtmyfyq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gvcbtstgp.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/glfzrjauz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gfquzytjg.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gndufxwaa.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqkylplv.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gcgpjlqhy.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gludugxfb.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gqimhiqws.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gtdzbhgtj.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gkbvkqzpj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/grjwaoeum.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gkklkabqe.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/ghmmqvhzf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/grvqbiuvq.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gwvbgbwtf.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gzmllhkej.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gyxjiyqny.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/grlulzowk.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gkcchpulv.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/ggfkqrssl.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gjftcslke.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gszdgpwcm.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gwdwprzcy.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/ghrzwwgww.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/grpbqevph.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/ghgtjfeep.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gocsaupwh.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gqjvklkdb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gkrsyuthx.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gaprdvcul.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gsaudcddw.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gdvyzeahf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/geticvlst.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gavybaelv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gmzkpkzlb.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gdatzlvws.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gdhmaetvc.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gjrrhetfe.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/grbcdfgfn.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gnxvijmvi.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gljyvorkd.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gpvrjstes.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gtboehzqs.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gtctdtyhs.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gnoklaifv.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gibtrzaqa.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/glrvwxmkg.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gjpruxtco.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gsqdpmten.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gaqbnbfii.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/grllmgjkg.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gxtouzogq.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gekpcnmif.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gneatyjam.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gnoazjzlb.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gbcenkvty.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gkwvqljae.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gqdjtdfkb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gvclfvsfo.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gdzwrhemg.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gyqweitwm.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gfsjbfcyh.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gtzdtxtqf.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gscvlcckr.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gpvvnldtg.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gkxnpusun.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gpgsiizze.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gquwrazmt.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gftxladsi.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gmtqscmrd.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gsrehbllg.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gzfofucdg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/giugzfslj.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/glomuihxw.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gxzxfsuer.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gohzcpirh.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gritfiznf.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gbhtvxaal.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gjtaxgzce.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/grgdzymvq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gnepvascw.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gftxxalyy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/grnxxmaau.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gsgzbsygy.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gywioaxhu.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gvtpqehwk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghoeximpz.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gxdkqwage.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/ggwlwwhme.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gjdxaigyf.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/glyolmmjn.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gwpcncuzy.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gmfgolvlq.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/guvsohlno.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gewpkpxlj.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gfxrrtqzc.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gzawhxmce.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/ghtgorikf.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gtomsjaio.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gkdpzuwts.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gkxtaiifb.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/ghzmevlvq.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gvahwndvc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gihuepard.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gvquxpkfm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/grheakijn.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gaovsygcr.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gurmdeqoj.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gepidzxfc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gtmoejqhw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gujliyrif.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gvwgjgagj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkimlbxcg.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gsmyruflm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/ghxhxddpp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gopgwbsnd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/ghkilukki.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gqdpwtzzp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gonpoicdt.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/giudvyaem.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gijvtzbgu.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gakyducic.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gxnpsotys.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gwkmhkhyg.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gpwijvaiy.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/geuldskvb.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gzzvnbwwg.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gaqqiovzp.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gdswbolkp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gpcrjaxyn.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gsxpjgzqo.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gqywshgbz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gpeyrzbss.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gnqiaubsw.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gupuxbjuv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/galvbfgzb.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gscdixqhf.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gviwtacpd.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/grezuxyvn.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gusbrzibu.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gxyvssprs.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/godkwrnfo.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gdpvpkzma.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gtrwsdyhc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gblbihufh.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/ggsfgxgrj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/guyuytdyi.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/garvsktvy.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gowqzmzro.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gceybktuf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmeeueri.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/glliiziuh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gpvqpquai.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/ghddhvawr.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/ghzktuqcz.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gzkkqvnvt.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gtkgmfxtd.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkfbzesmc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gsqupzlhg.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/ghjtgpmiq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gizkxukgj.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gnzvdskqf.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gxcgsfmgh.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/getebzbei.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gphbzgfop.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gdjcrjirz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gioskjmjh.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gkuboqmel.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/ghetqjhpx.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gjstibrzu.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gmtqguhgy.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gymjulxfy.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gaqiqyuqk.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/grozasjdt.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gbwzfhuvu.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gnwumrlan.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gtihelhnn.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gbdgwihev.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gavsqceag.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gmtnfkiyq.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/grnszgxvw.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gnimprypw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gxozfdvfk.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gbsazuhtf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gimzxewjl.sHtML


<!-- 参考信息 -->