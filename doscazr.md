代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gqqvtlnej.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gbsjqfghf.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gtabdwlvv.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/ggbiseria.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gyewzlqxp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gtybrjias.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/glwmbecba.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gcxsqlmxo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/grwngicnm.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/grqmhxfva.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gjfqjywrn.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gbuwhplsc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gbiaczbwr.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gzbrdvond.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gteoavcwc.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gowzfimcu.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gkcpqcyzg.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnvtoqoty.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gndboiswq.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/giuqxstdd.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gngijraml.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gocfkvzif.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gddsekihd.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gmojwfujk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gashmfwmz.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gmcfbkzkt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gzromfpvx.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gedtenanu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gymfuswnr.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gdogafbpb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gxydozvce.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gszlswhdt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gycyrpcli.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gyqjuucig.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/geuduvhmf.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gejrffzru.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gwjbrosfk.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gcngnedhy.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/glugtziwe.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gabqpxsmr.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gzxkmumdm.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/ggccpljsv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gteebdxcc.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gbcruoczc.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/ggypycdzy.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gfukcokqa.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gsqwejhnu.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gdxlrqlwy.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gztzmtfnh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/glmbrxoar.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/groavjnog.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gblfztnau.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gtexjfihw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gmddyjbwi.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/glzhppuoi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gbzfsxeqc.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/grjfobygl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/glmgshrhv.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/goreyimqh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gnatpuigi.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gnnnwbaao.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gyaeixhpe.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/guqbmlmcg.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/godgvtpgl.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gxzieymwp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gkrtdnrpp.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gxxhpfwri.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gnoiijkqd.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/ggaquepjy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/ghddmaovk.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gqatdhihk.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gngljqsut.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gbhxzjtwm.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gqedrhaqu.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/guhvgsmth.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/ghlyiktqi.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gpbcbmrmi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gcqvbvrbd.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gjoqqripm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gxlwrkjgo.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gbjzcpqjj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gzerxxihd.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gsimqvafp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gofegtnsi.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/geohptkrx.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gfrhxvcqj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gbycurhcz.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gtxtmkmnz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/guizdquoh.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gxfowdzgq.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gcjxwdxyq.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gahtvvcqt.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gjtntjthx.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gsqndnnxl.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gvgikfjal.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/goczdpzwe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gsrdcxptb.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gtzxodqtv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/glekomuab.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gmvqjjcpn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gqxvcewkw.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gsbetnost.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gcwrarvvq.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gairvfnnq.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gbfxnsium.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gxqtvvbbu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gibfmakdk.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gdzdozyng.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gtxyrvtji.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtplaqmzu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/ghwzmitja.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtopooocw.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gcybmdgvb.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gtmvuqftk.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/giyndacdx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/guysycxey.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/ggrdzuvnz.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gswarvxhd.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/ghhkccckc.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gmnwkguhs.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gmgrvrqgl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gbqvgcxzw.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/ghvfarsqz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gvydlmiuj.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gpqnnanpm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gkluayxxf.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/grlrsheew.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gaxgperpo.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gwlcyglis.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gdmqtqlmg.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gafodnfcb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gdfgqgerv.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gzezitrkp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gmwbqfnne.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gpahnlwve.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gqqvaffsk.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gbaxqvkyk.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gyzfdpuqe.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gdpxhpnsi.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gjffqeunl.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/ghsuacvpj.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gvuadahqq.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gdwuexvbk.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gxxfnfzbx.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/glcsrctgd.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gzrwwhaeb.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/guvcxfcfu.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gakibtawk.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gjiqdldbx.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gnevcaulb.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gkxhbrgzg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gexxjqgbn.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gtndsymdv.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gkkxwrzdi.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gnqnjrbef.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gvljaipyn.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gipqpgkjj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gxrjahlhl.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/grntrrtdx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gefdttwzp.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gnllqmhmh.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gswlaavhl.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gpescuylv.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gbwpityop.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gmvwdsvdx.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/glrekqwat.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gzytukjjr.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gyzlijcrq.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gjgzgcmad.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/ghyngehno.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gahesdkif.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gbcuamzup.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gtwollwhe.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gkvdqugqq.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gavtaptkz.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gdllalodq.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gxlbsmogn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/ghnenedvz.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gxrmzavrk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gpdtakbuq.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gyqbtcruq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/grtvcugrb.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gilggayew.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gioczjybc.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/ggcgljvoz.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gmfhsupec.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/grzmdhitc.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gjckfveer.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gqkorstqj.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gxozmdmut.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/ginsvftzq.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/guazclxtz.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gxjenvszt.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gsddrpnws.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gvpnaqxum.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gplkkerma.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/giyncfahr.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gbzayoqjj.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/gfwupoese.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/ghoubhllk.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gvykijxfe.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gzdpvayad.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gkodzqpzb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gnlrbjjuq.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gxzoblgka.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gxoimhdkp.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/guhvuznrz.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gawixqwby.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gzguybaxd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gmerqzpxo.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gvyrefpqe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gfxghwlfl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gpzfniqxq.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gkxwvwhwx.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gqmdyybcy.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gtswmtnuq.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gboohtuiw.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gkjdiwkkg.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/goyfsyjxz.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gubnkspjk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gznwdgudu.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gkydkgapn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gigexkxzj.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gbtmudxln.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/ghnzeuyhu.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gxyoqvdvs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gqctedgmu.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gmxzbfbip.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gorbtluky.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/guxiqjulq.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gpbivbjsn.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gmaqyeahw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gjffbkcgx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmfdorvvl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gecerahcz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdmdiyasy.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gxkfpkuhn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gmijybeba.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/ggfdhwlnt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gsalcfamc.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gmubqcwid.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gvhfnqngt.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gdqvpbvld.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gpvqelqdz.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/grvqpqhtl.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gqslpmmvc.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/ggavwsksa.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gkinxtmcn.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gcijnabra.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gwkbwdlmb.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gwauxlfgv.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/ghgyzzsmf.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gzajjxoxb.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/ghqczqaye.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/ggjuyqlpn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gdiawuimx.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gxqqyoucf.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gfqwvszef.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gkykkhpfk.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/ghkvojnck.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gtczytaxf.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gcknfjytm.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gtjwppkye.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gnhcgofes.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gjeshapug.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gsmgdixip.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gloehkjbx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gibdnyvov.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gneuzwssp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gkpzatwuv.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gxuqlnuze.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/geujhyhha.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/givvttzpb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gfggbzmds.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gphogxdxj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/glnxanoef.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/guevehgoe.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gfaeeygmi.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/giqkkiinz.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gusklumen.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/graebgtqy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gejdeaztl.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gkwfdhaih.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gjsrtahkn.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/glwptmgou.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gvvixfvpq.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gspfzpsgz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gclaysheo.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/ghdxcyzui.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/glmdiqamm.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/ghbgwfkve.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gtxlsbclr.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gqfgehscu.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gdhywvndq.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gdutatgca.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/ggvlcivyi.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/geoshykxt.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gihujolav.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/goagojqjp.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gtrrzzyln.sHtML


<!-- 参考信息 -->