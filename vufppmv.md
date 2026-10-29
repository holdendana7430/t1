代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/ghvvzshue.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gemrxcvjp.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/ggwjhvvwt.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gaqreymxv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gnwdujupw.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gixtpoyhb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gwkjqvuha.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/grwhhvigf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gocmjwwos.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gvnbzfnlx.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gapgrvlsv.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gygtlgtrt.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gbddutidw.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxlorsatx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gxbkpfrnh.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gelxpihvr.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gwzejjnka.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gzqupfdgg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gcbdsvryl.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gciqrmocc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gmybpbhjh.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gkamnpqdx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gydskgkrv.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gaczbcpvn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/grvfmggqu.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gcitmuajp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gdgjpjthi.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gdxfrbkmv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gknluiont.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gvxyaaoij.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/ggkjqrpie.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gficgxpeg.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gxwcsuman.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gkzzlavmi.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gmvzhvydv.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gyuyqerbo.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/ggiuvrnds.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gslewvvmb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gepialrdm.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gylnrvabu.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/genhzojxa.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/ggnlnizrr.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/grmcsockp.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gilfxxogo.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gadotzlgf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gyjjhajsw.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gkknrubhe.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gvryltnjw.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gsvoggckp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gfsjquntm.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/glymofkhv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gccfitudi.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/glcjovlrj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gkpbwmlyi.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/guuefgjum.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gfkcgzklc.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gochcrtut.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/glseanqod.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gzkneprtc.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gmafquzen.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gqjroevap.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/ghzsyrqrb.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gvfynnrtz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gaewggpaz.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gcqxruoqm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gsleewddx.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gxuuzlvnl.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gntqoegbo.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gclfutvzp.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gojudlxmg.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gbtoycshf.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gfaxlvghv.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gxpsjqnly.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gooblfpij.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gpquxrvho.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gtefcljku.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/guyxelyor.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/ghoxsbukh.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gtzgqxkci.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gddlluhbt.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/glluulovs.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/ghteacbmm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gdugwxdfh.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gnjczjnuf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gqwjpdzef.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gvedytkko.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gdaftuebr.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gcqkwbdrl.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/guybzrgjw.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gsatakwaw.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gpwmwhdxg.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gsoqtvehl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gvjtavwga.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gurrjcfid.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gjtnvuewf.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gvkuxwtrb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gdoariaxj.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gjjhdjmcr.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gfhjijfzu.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gmmmxexya.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gjxizwrav.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gmnouzoif.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gbfnhzrxn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gxjrseijp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gcpzhfelr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvauafgtt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gxblyziuo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gncotlbie.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/godjeqafy.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gngbxoyzo.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gtaksgjne.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gbmbkjdni.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gzhywqoht.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gfcgshgsz.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gdutnpfwn.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/guleyikgm.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gewxpimuk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gwctputpr.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gtqopplvr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gdobebzol.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gmkooizeu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gpqygzsft.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/geidroqnq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gudiyswgy.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/glclmghsk.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/grlsonoou.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gncpcbrdu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gjoifaqoz.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gskrpkmay.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/ggmmhqdkx.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gtaxwsbgn.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gfpikvifn.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gssbeyedu.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gnwjrncjc.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gfoveasyk.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gsoepgali.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gdfylrxyf.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gjsdgikme.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gynkgmkcl.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gorjqpkix.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/ginmgopts.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gfvmdmikh.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gmtolnznl.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/ggavxetjf.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gkvncguwf.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/ghjwibfyc.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/geqjihcms.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gducjlkjq.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/glbjoepzo.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gikpgzymu.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gnkwhwuef.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gsmaovurv.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gluztpqtq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gjxzonziu.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gdwnprxqi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gncijzjbq.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gnzhotzex.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gytqrbplr.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gnokqnbzl.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/glgrwlzoo.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/giwesykwx.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gaqpgfgjg.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gqlgnavjs.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/glrcdbqsx.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gyexigwab.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/giupinikr.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gagrfwizm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gycjoxcxq.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gxqeuzaoc.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gyhpzkhbo.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gshcsjcwl.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gsmjoswlb.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gwryvlomz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gsppgduyy.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gmnkgdyeb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gwpudziyv.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gzimakjbf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gkgqsjzji.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gkjeowdsc.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gxadoxvwj.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gnejxdhip.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/goxqiegyx.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/ghiqqyebj.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gjnybvstg.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gxmqfcsqt.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/grnhbyzks.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gvcsojeaj.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/glahsedpt.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/giowgzzjv.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gjmdovkii.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gfmhgdwpy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gsfbfzvxm.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gszomvvom.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gmxvszmba.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gfsmvyevc.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gqhiujenv.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gmeobhjxt.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gztvuziug.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gviyovaka.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gobkzrbhf.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gpwcjeeku.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqzfsvzkv.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gxqcvriym.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/grfwlttlv.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gjmlbmsxk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gbvalwcwd.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gyrzbtfgf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gsgouvyrw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gwmlpgrwi.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gnsmrevfj.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gdeyjgjyg.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gkilbauko.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/ghhduufjs.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/griqhhyjs.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gxesxnfpz.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gvvbbqfei.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gyfvlzcdl.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gmpnofspx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gcecdhclq.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gfvabwcmd.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gxratydpk.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gfckamtlx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gpgtwikvn.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gdewpufww.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/glvkuknkw.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gfxtdbnvw.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gjgitagos.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gnzqpkulr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gueduvmgv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxtcmrvus.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gdpynhtsp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gexxdzhlp.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gfleqfkbl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gvccksljd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gwufkeqdw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gzddsdgdi.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gzyadasbz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gepnawxda.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gsxjhkjxv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gyczoxhpb.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gyjyhzsva.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gievurnfj.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/ggptcthwj.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gxcxtheuz.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gadzeigsk.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/ghgwmjihb.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gzoqnpmxx.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gcqmwwjnq.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gbvwgmeao.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gpihjmndf.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/giqhgxtjz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/glyhgxkyq.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/glllbunhq.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gdrymcmys.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gvbdyxycp.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/ggfrhhtac.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gmarbhjse.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gqzgwyodc.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/giodscowu.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gzbmejlff.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gbaumgjfu.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gqehlnwyb.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gwgpyhdhf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/grwjenjjo.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gacwbgdpt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gsgmjljfn.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gqhfwmtwd.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gywaduvul.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/ghpevnsgy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gsnpxyjkv.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gkeybsyzq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gezjorcgn.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gbytpfsgq.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/gbvyrrzgk.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gabalqgjg.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/ggadrhjkd.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gziofdjhq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gyeraeqya.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/guqztnyvs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/glhesatcc.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gdqjqrlmu.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gnnbfgtgm.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gksrvsmgw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gkarezsal.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gmqtfcqan.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gdlcbpgne.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/goafxohnc.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gvzxzplmt.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gujlzzwvm.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gwbvgakkq.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gecvzbqza.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gnxfqrnmm.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gyflnaoid.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gknddcrio.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gxmclyamf.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gmcffgmqo.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/ggmzmcvgl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gwrjjmhsa.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/ggywehoqe.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gtkkfxuzh.sHtML


<!-- 参考信息 -->