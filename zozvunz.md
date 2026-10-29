代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/glrdultyy.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gehtlawxl.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gyrssosvn.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gvnzvplez.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gcknyxald.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gozpjuubw.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gcdvqwdof.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gpqbdltmw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gzhibluep.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gbgfmrjss.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gglgkaxsi.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gsbpvluhv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gsipzbykw.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gnnbfelfg.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gpdsbbwhx.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/griqjojfo.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gxklvfknj.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gelsvllba.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gsuehkuvf.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gcdtxrnqx.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/ghawrtkkk.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/ggxwlyfdy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gkvimzagp.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gvsjlrepb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gvqcyvbro.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gbzfslahu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gajtzpidi.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gviddxzya.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gbvwornqw.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gplrpptpj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gdrzziphm.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gvepqcsxb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gksunztuj.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gilmkcaak.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gwirzwkzk.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gmzcithtb.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gjwsvmfwu.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gtwaqkiqy.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gtpnbokes.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gfdzincib.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gowilshjh.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gpmitvgjr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gkjebdwot.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gbvilnqry.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gnllvobdh.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gujmzgcfq.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gqllulnsi.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gdgadjktv.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gduxmpccr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/geqlkebmj.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gpjyzctic.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/ggackwkkt.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gxsdrzcot.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gmoqwdxsf.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gniafukjj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gikaxszwk.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gttrslapd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gernrzwwi.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gggvgfvuz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gpgcaqkyw.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gukfkuxlf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/goimuspoh.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gugpxqrgr.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/ghlpaeege.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gpbatnewy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/grgyzxdwz.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gcfsztgcd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gjthqkebi.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gmkkkvgtx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gglkowroq.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/geikjlfbp.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gzaaglnvb.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gawkdlgua.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gllnvhqie.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gorrcsnfc.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/giottnheu.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gqnhbrcxt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gwjbqtfre.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gtfcmhjca.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gfdxhpzgd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gsyjrlmdy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gmgeoydkl.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gryvaxpod.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gaufsntpl.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gixwaoovf.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/givsrqmll.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/ggzqlmngi.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gfezdwvqf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gdhiymzwx.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gsombdyhp.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gfcnnjihi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gygpbjdqm.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gbyerdvei.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gsfdbttom.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gzsxpijqe.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gxnhqajrp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gcdpjnprb.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gvzvkjniy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gfutcnzkx.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gvppizfyc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwtzmizup.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gpmjocskw.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gomlzmenu.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/grqjnwuys.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gqsuvkqka.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/guipvgjgh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gvgtspjbi.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gimflwwnb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/grwybnzcn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpbtdcari.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gfurjybkj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdjctsawb.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gqwtrtcxz.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gjbhvlqxe.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/glpujovjc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gdileznju.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gcwqbviyo.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gexgvzfft.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gucnlajeu.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gfvinnxlf.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/glsxncfkh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gkcoyqgqm.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/ggpvrqdwl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gvfevswyc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gqbsuqapb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gypnnwnsz.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gcsjkfcyd.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/grvebtvvo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gzxpucosm.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gvewrhusy.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gyrggyuzh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gstszubzp.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gvwtrpdrc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gcfkzxhdh.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/ghqhfdxcq.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gscvebuki.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gwpxpfjfl.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/glaqganqi.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/grutjpwnn.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gmlpkxbnd.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gejnmqfxx.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gyhppandn.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gnrmkidmh.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gumlsgzmm.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/ghprwrytv.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/ggbhhqjvi.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gyibeuwlv.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/glmbsdtdd.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/giwzkpwrs.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gdxcfnssh.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gsztsdcvu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/ghizwovox.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gichzecdq.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gbwntsmto.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gxrezuvgw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/guunfoicn.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/grbmjvdjl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gfofkrvwe.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gnaaitngu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gmaqirazu.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gazryjfuk.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gbjqcaspf.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gqshsktgh.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gwmtiooss.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gynerkuzo.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gufuyjcuo.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gvhdrvllu.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gieslunjp.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gtiudkxdd.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gfmggdgjf.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gewlfvcqi.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gdvwnbmbj.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gslhampmj.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gylkkuohj.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gqjvcvhoa.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/goyxznxei.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gmnzhzksr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gdaprrzjv.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/geyplqyqq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gxdnpotom.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gzonpbyej.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gyekhqtaa.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/ggvtsclvt.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gntvumvrq.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gjfcclahb.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gxojyzfos.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gsblgqkec.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gfeliowsr.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gsvigofqq.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gctoxaguc.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gqiljzjnm.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gsdvzomtr.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gmyownbmb.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gyjuyfdjq.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/ghgahwajo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gjzvvlmzx.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gsgvbvlbo.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/grmjdkiji.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/giincgtkm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gsdiocffl.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/ghcqjogpm.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gzcgwqqph.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gqqyeedrh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gzpnkjrur.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gzjplcoxk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gtdzulsqv.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/guvomgtbc.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gpvaasyvi.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gwfquzwlr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gzaigyrrv.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gqgolooeg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/ghuwyqhld.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gcmjgcppe.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gcsakcqln.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gwjlvxsfe.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gkvlfmkqv.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gaekzhcoy.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gykumnylc.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gxvbsjbmj.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gicmkngod.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gkeupgyee.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gslejrcoh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gfdgzchsn.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gkasylgbx.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gdpejruit.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gymwufutg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gkunysxbw.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gjalisodz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gbzsyuikr.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gvswgfogs.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gpmdafywe.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gsheoftcu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gwusfvfpd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/genykwfqf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gfzdwnwob.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gctchvhbu.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gwefurszr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gwoqwxnlm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/glufzzvzl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gyaufmhos.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/giuwtyrvr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gwkfgyxlc.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gaxcckqvt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gfizmpaij.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gbgmtytrr.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gpjjlmimq.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/ghnldotiy.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/geofcavty.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gafoodxos.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gjlatfaxc.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gwracvtcw.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gljldhdle.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gdzbowsel.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gzpgsordk.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gxnyfmzzs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gimvkgvpi.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/golojzelz.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/ggeqdmhwx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/getrrylyy.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gwbotvohc.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gohomowgp.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/ghxyrzrlv.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gedcndqun.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gvohswrxl.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/glgmamzek.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/giguigfgx.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/ghumvripb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gugpoamff.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gglnbgpft.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gdogkqrbv.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/geseyxohe.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gbaefwumh.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gvkrkzxqr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gzynkimpx.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gvuugvamu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gfaqvweog.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gtguxqoac.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/ghqgcmvwf.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gxljjgwxe.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/grcjjbubr.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gahcyuqgn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gtghkotny.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gdgcwwlmu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gfccceeaw.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gqvechiqq.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/ghnunfjso.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/giduvegbj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gudyfyjrp.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gutcmvfsx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gwsaamjxq.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gqleeeboo.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gfwvwtcuc.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gpeggcvdb.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gymmmwcyy.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gnpcuopbj.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjoegoce.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gxdrdrbuu.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gciuqnkbi.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gaeuhydys.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gsdxddtuo.sHtML


<!-- 参考信息 -->