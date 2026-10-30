代发 wailian999

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecbcydqe.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gyczgjnai.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsggiicun.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnpmenul.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gzpkjyxuz.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gtecqlrza.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gqomkyhxx.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxebwwbh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gukkqbgrb.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/goxjzyrjy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gxvqzsbeg.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrhvcmtv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzzwsrvo.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/girzjnjss.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gxcypfvvw.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzlftiyy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/glrqwrisk.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoygxxuh.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gieopfgha.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gsobnudhe.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyxiyaci.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdsffmqu.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gandnjpgc.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtuzbljyt.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeilpbwk.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkdhanii.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdjuhvqf.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypaydqag.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gcgbqtocz.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gokhmvgan.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqcnhdig.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gaxrtpiqi.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/guhrelnei.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giisjtqsr.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gjxbtxkif.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbvkbeor.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gocnnxnir.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gnpmzynzx.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gheasuxai.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyofxtrdc.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/ghnvrxggz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/givyajwyq.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gavhlkzjt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gflhloqyk.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwyqlvqo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gkuqhpofs.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gywevvhom.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gvdtuiqid.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gibfamdjp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gtftqcfkd.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/grqekqoac.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gkxdbuidp.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpcufkyg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsragunc.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpokabyei.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gviwbscps.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gswyzdnhn.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyikhmpw.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gaicostba.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnrmqtjk.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giugwcbjc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyylhnau.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gwnrgzobr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwxceshqy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzmlbsps.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdhwaywrm.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gahvtcrsh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnwtmxwp.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrqrptot.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnzeisxm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gojwshsnb.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezwkgpaw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gdrhvbase.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gpkknjndd.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/ghxbjiatv.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gkuirrtej.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmawnzcnm.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gngpvozmr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvhckwva.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzqofkxg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxweatgb.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqzutrkf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gqivtaqil.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gbfmzqhbm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblbehvyw.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gztibyaqg.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gzvbnlakh.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/goxbgbbmb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqoutpwx.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gwszjhsab.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemimejfa.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqxtzobv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gklgbbfbr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gteyijzjv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gspwryhjb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcsrdkzjn.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gbtladvnl.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsnhyefc.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyewloncs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gdvfblclr.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gepixhoru.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubnrmlcz.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gmiqwwzns.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhiewudo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfaimske.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzztwqfo.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtvxxgzg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gnkrkfzvz.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/guzknwzvk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gvotosuhu.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gdikvuurz.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gjesltvpj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghokxtdoq.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gvdyglqwv.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/givtfdfyq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gdhsghfmk.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/grrhppwhv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyoaekwm.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/greubzxxq.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gncvctdwr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwixylbrg.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyiwpndo.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gznrzhjfg.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gxsrcgvya.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gcmfpspgy.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gimmcrrte.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqfhcvtv.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsioaihrq.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxozimnoh.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gycztlghw.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzbzfimv.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gibashbam.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtfxbzzz.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwrefsks.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzsmwcxh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/ghrjfctln.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/ghldmtclu.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gturlopln.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gwopmedxa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbfdjuks.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwiitpygi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gcynepgmn.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gjhufmjuy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gephumoyb.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gfductrwy.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gqzanzkqr.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnhyuqkf.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvadsrbw.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/grstykizw.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccoyduuc.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/glalbkeok.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gveecieiu.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gygotknxt.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/giaoxfagu.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnzfwths.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gjpsakfyy.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gyxpigfae.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjivibhgt.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuncrenf.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvarrxbt.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/glbvoxpjh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvjnimdz.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gnqhjtqzm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gumfzfcvq.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkdesyfk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gpimcmtul.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgsbpylo.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkqthyqu.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsnccsgn.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gkndhonln.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqkuuoln.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gogbbbnoc.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghurhicxh.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcqgoala.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gzzogqmbd.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gqfijakgn.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/geufmeuzb.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/glyrgrale.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwxekigv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbwjegfc.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gtucotsha.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnbczvyq.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gwcuavvsn.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gysvdxlaf.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/geaaeepkd.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpdpnbab.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gyrobshmm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyoshjjxu.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/ghprmoscz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshnjmyla.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/glizdenfv.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gvjwhgboy.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gchepfbez.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfcrdqxaz.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtzscnvqn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqmdhiqb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzmzcsqly.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpibtbhd.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzedxmpjh.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gerlsesou.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqrjtxuj.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gqjgnxxgd.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnldhgrh.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gwknsjozd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gublkifmr.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/geyubaogz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfbtzrrn.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gqphyskga.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gezcnypvp.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gpuqaihwz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevwufojq.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gwubxcxdi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqxaxuie.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gnpmkkujw.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gadjulveg.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gckvoffxj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsreiljw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gewfhdttt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/grgdsggtc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdjcgduna.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gcikrwcxh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gravjkprg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gujtrkiqo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnyifkbtp.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmazhhro.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gujgoqfkk.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcmohqgi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjlnpxjy.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskplxnys.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gilwbgzoh.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gozfgbmwj.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gafpuresq.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gsieodzud.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gjlulusnj.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gjczdfqus.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gthlhfhcx.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govhaeynn.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfztkmmod.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gauxsdhaj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/grcbjcjpl.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfegjtrm.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnouprat.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkxbdyub.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzjqegak.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxthyqjys.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gueakymor.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gkduraggh.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gsycfklxk.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gszlrcpze.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gogddasza.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gckynvbje.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyhksfoe.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbjyezqe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjprvjauh.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkpnqzsh.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmnvjwhg.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gssyctgxt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gkcxfnafn.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gblbhpzgc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrsuppps.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gvkkistuv.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkzdqtvu.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gycaqmwne.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/grtmklbev.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvsdltdyq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gwkdnyytc.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gsilbnonm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gbdkbtpih.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gkdylyfmo.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgwaglof.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/grubsbdcx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxmmscsl.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gieagcgne.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbptdcln.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gkrtgieeh.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwmmhufe.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbjerqqi.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/geleecokq.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaaqvjzb.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstyyunjg.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/grkrtnwzo.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gcsrfbkby.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukglcbnb.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxoxjxbe.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gwndlhzoz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gakqvqxje.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylpxkpro.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwubpddnz.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gwjiczhkz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrtrrvvj.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gwonmyuqw.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvorgpggl.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkaqknxb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljhfqhcz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpqforns.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuxiolrp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrrbgemj.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/geuszywwv.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/ghvuegvwo.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeydkfhm.sHtML


<!-- 参考信息 -->