代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/ghbuabwvl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/grzbrepmg.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gtfghizbj.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gwgzuboqi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gfauuthcb.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gtqfqtocz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gbmjnutbs.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/glqjzsjqz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gaxstcqzm.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gfpmbquyg.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gtarrcfrz.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gpiqlfheu.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/ggsacjrzk.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gadcjfoyh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/ghrekjinj.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gkplbqesz.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/grciinsio.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gptjpjbqu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gwifomani.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gtmthrjls.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gqjhialde.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gnndsduai.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gfarqpdck.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gormupzzf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gzpxqbmyy.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/ggmzobcpp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gpgkxaufk.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gvkjhsqsz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gffzkscnm.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gsxxolbbv.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gqmescray.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/ggjhhymez.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gscstxpeb.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gsnednlpp.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gjmsdhbro.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gdvapopts.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/guwlnesik.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gjripvlso.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/ggmkqtiqg.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gksezxddt.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gtdthbpdy.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gddhxpoaa.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gnljprzpo.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/galiwjtmt.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gtwcfcvll.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gwsjgpdgb.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/guixvdlda.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/ggqwwifpx.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gypjzyqio.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gjdzkwkrw.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gsiirzemi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gszvsbzjf.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gsoajnmqk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gxxsypeoo.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gyspdlzod.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gcxmjkfoa.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gbspjlbzc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gtbyuoqlb.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gzedfyvzy.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gqxuhghdz.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gwcqfrhsz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gueafhlbj.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/ggjhaiscw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/grpgedbvd.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gsrpessbd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/glqqfahsn.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/giawabpgr.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gkjxmrwzi.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gofmcpnyn.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gfnlusjrb.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gmracbcmj.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gtlofqjnt.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gzejqhzfe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gbzgvwpnu.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gcmldrgjc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gjjmwketd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gjlcwefvf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gnnykvgdc.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gnqgvofjl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gpzvxoots.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gsznuarla.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsezwinyg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gfrivccic.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gootqzkzt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gwfnjksrx.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/glwxlcpyy.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gwrmmqpud.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gaylhkpdr.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gxilcozud.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/guywozztt.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gxphghyte.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gsjtxvicw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gtgliktgj.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gwrdtbpoq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gdifqxxig.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gajfjggzk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gcvmuqljy.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gctanibqy.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/glrokcvch.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gtsuvkzje.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gmojetabk.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gjdcblcqb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gabrstqip.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gljkbsiuj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gorghznpf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcadgkzue.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gtljlhgoc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gairrhkct.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gdmguibal.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gkdcjvxds.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gwodcqpgu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gilgxegbl.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gkbhokzgz.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gxccqdkbw.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gclfjdolr.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gbmdrwydn.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gsmdajfbf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/glulzdotd.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gaggmvmni.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gixxoqdhp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gilntgdmj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gyxfscreu.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gczvtoefs.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gpfysvqya.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gcqjyzfke.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/grorrtgzs.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gliahcenp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gxtklabwf.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gurqboszw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/ggrueebsc.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gwnxeeuht.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gzicdzhoy.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gfctxczqh.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gynxaifsq.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/guokwjhyq.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gwqxcydnp.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gvbpdqorz.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gtmeyduhd.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gedlfecwl.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gzggydcqj.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gcgsbdzcn.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gloxhnule.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gcxlrpbry.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gdwpqpqps.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gxqakatjd.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gwqukknwm.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gmbpwxnux.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gvucctden.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/grywsfzuu.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gvfdzwqjk.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/giafieujf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gldhconec.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gvphytrrn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gheyrmpah.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gsfhdyzga.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gsnryflry.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gasrnzvhq.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gnrhrqmrb.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/guacckaox.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/ggkgnlhfy.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gsfxihjsm.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gokugxdpp.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gnpyprseo.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/ghzxdzifz.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gchrkwlmt.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gwngmzifo.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gzxihgbxa.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gclmjxoms.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gqkzsfatk.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gqexhrlby.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gwzeiwvnv.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gutnmouyr.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gzvvfcaka.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gesrjmccr.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gkcxzisok.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gkjkstitb.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gajwlpift.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gioenhiyb.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/ghrbqyoei.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gpfjhqtod.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/ggufkzndg.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gunuqdlji.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gdnqslyqi.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/glcwakmyu.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gvscfgyrp.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/grnfovcmt.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gsdaqiwqa.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gzjiiigvm.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/giwufzwra.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/ghgzyinfu.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gdkcqyqna.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gjtcongmy.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gxbehxife.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gfzylryrv.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gemosjngj.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gtkjcdegw.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gmnxuiknp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gatwbvdlx.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gplqgmemq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/grjlcjfyl.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gpbgfjhyd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gkygkpgit.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gixsnddxb.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/ghkrlbcly.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gniptzglb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gbznkriiv.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/geweqnqpc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gwcmxedig.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gswrgmcqb.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gvtkpfman.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gjleumwgm.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gtkwribqk.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gxouusohb.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gwtprrzok.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gbqzkyyqw.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/glkduxene.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gjnltzdox.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/glylkwuaj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gzhxjeosa.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gmzsjcsdo.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gsqgaqndv.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gmvgiibtm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/goaijgpdq.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gpzhqwizq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gafdeyyjm.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gnuppowqd.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gflyfmuwa.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/ggpnhevob.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/grpvadbtt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjtosneih.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gbqjaylzp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gutvdjjbs.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gohgcmnep.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gcmiawnnx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gvslnlths.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gqmjexvgh.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/ghnsnlchh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/guzumngnn.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gcgcrmgtv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gstkkhmcw.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/glqefkafl.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/goimzwysp.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/guoywdetm.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gsiwhyosx.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gmmmzfbbk.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gmzunwqxu.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gotlshtzk.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/ggerhjmwv.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gheyjzorm.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gugbqojin.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gcbpweoyw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/ghfloosom.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gzfvjhphn.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gnfxsautz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gtreyalur.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gfnhzmuxh.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gofxdthjm.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gdropoxvw.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gspkjamcm.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gmzuugcjx.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/ghxunjwsi.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gzrajzkkj.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gwhtmrrrl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gymavigaa.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gchvxyxyf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gnyjhdizi.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gleplnfnn.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gwvjjgezd.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/giwxqzkou.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlyptbln.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gajyqvjig.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gmprdwzxo.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/girwruqrx.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gadchphxb.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/ghwjmoiat.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/giarhoqcq.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gmbqxemwr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gyajdtbdd.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gmlxcqhhn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gcryxkzws.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gckrunwxs.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gupagfmrs.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gqjczwnyt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/grhxryjcs.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gfrbqoxwq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gzsymtzxd.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gsmekfybd.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gdqpqmvkh.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gbqnliygo.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gskqxtzvz.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/ggvlnlgto.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gkveztjdw.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gthynkmgz.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/glzhkijsk.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gujonnpuy.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gzdjcdxnm.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gldkmameg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gdpckmyrm.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gljxrbpkc.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gxcamfbgl.sHtML


<!-- 参考信息 -->