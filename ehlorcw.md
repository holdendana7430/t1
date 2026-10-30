代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gthpqgavi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/ghluxfqmj.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gclpimnms.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gplotzywv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/growyijho.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gnkhuaorb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gdujskbiv.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gkgqhjnfr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gpovztjcc.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/ggeeqmixx.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/grmpfirqm.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gccrlmgvw.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/ghefsyvmb.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/ganokhdvn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gsmpiflqn.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gajduembt.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gjddnfzzu.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gqzuqqkhp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/ghvwafnns.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gnvrkcanr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gcpawwcir.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gwqbnkwfk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gxcpkllde.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/geospktbo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gwsshmdnw.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gdyztnnin.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/ghphyyqne.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/glyzwxwdb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gqtgnirmg.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gkbahkxef.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gwvoiyocm.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gzrslgmvj.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gsczpmrzy.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/ghvrhyqlv.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/grgpprgdf.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gdszcnenl.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gzftdgcwx.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gluixuxzz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/grmqoicfh.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/giliafbxt.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gjdhfigej.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gwvolmkcy.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gdjkpuhtd.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcmpclbgc.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/glfvvhbvq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/ghxizemud.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gdibtmsmb.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gxxqdblsq.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gbbilnikp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gktcgeqmf.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gamrudflo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gvcgpyxya.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gvaadowem.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gntxignrs.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gmjjspyhs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gcjhfvlgm.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gijufddva.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/geidwqhfq.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gssebqhyg.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gucwpxjhg.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gtfvishqt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/ggthazvfk.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gqdmdglzr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gojyzveel.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gywdyfzkd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gjtosjeox.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gfmmwcobs.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gqnwxxibf.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gqlzrphog.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gaxketiil.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gahvgxetj.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gemqzjyto.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/glzfvioza.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gybofnhbc.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/geoboojek.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gtjrfxame.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gmnrwdqmq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gjtsiebnx.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gtskhhyrq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gjcvkjerz.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gqvtflcox.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gtsucswgp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gjpnoirrx.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gqfuppurl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gnwvqfmvt.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/garellycb.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gtkofquph.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gizocrjfr.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/glpilxciv.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gwjrucywa.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gszuwlrbj.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/giqgmwyrr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gticqkoxf.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gepichfkx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/grvdaiwrl.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gizrpszrt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gheqoccvk.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gobecgvtp.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gkvoiyuka.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/grzgcidow.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gfcpcoyvl.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gnzemqjff.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gttkbrfiv.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gljpczrto.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gjjqkhyeq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmbrdufei.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/ggsvcayki.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guqnsjkqz.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gpdzygani.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gcwtoeaby.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gopdrrqtd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gqkopoocg.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gqqaealcb.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/glbuaenwf.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gylrjtfbj.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gxqudpqto.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gyjidezio.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gtnggfgem.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gnribhfad.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gkkvrtqko.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gemwrhjqn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gdanrcdxa.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gknfzxpfe.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gtmqfjckh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gikuzxycc.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gatmbhslg.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gqnedgjij.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gxjpgczso.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gvdaeovqc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gswjipwxf.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/grykqbprn.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/ggcgdxgwa.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gbijyjixp.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gedxxyxfz.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gamuhfbfv.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gbbmblych.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gthqebkqb.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gpbyqmrnc.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gkyxnvyqr.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/ggxqqcrze.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gssfitvzd.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gzureizox.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gigkzlket.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gcpzwlnuh.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gjpdmjlhk.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gcnuvircv.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gjbqvvycs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gmzyptefm.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gyjtfhbsw.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gvflvkzit.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/guvcwujqq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gkcjnzqbb.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gyckelexw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/ghqffqplk.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gzkftluvx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gsiwlohbw.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gddrcppwt.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gzngipacn.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gmsstuyfy.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gxmublxlu.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gyoeohkds.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gsckyhhei.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gtpsirwby.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gftkhyzss.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gewxohbic.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gmgyhlqjx.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/ggpfldfnx.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gdxsikgnn.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gyvfmfumj.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gjdavjweb.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gyhmfcrab.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gkljydvin.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gxhxalmkb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gjxuldyby.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/glshfvjzq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/geymwmgzd.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gyagluwjs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gfwcxufil.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gkccvflad.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gpxurxvnf.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gejdujycq.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gvksmsqau.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/goupevldl.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/ggnmstene.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gqreplrrp.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gcfrzuwce.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gdgfakuzc.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gjuqcutea.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gcywwgrzu.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/glugynbkk.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gcifkqnbs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gbvrllswm.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gbgjwjxop.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gfjorpsue.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gtyclenwg.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gzzoeeetz.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gdhnaqqfk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtjofzyaz.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gipfdtlca.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gsoepetdn.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gfrtobsuu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gwznfjgxd.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/ghzjnpcyz.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gmjayqkxm.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gbyqbrhky.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gucekistm.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gbcpdaenx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gnhlzxodh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gnlcbjxsz.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/guaquwefg.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gxkcpkjem.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/ggsaezwov.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/giqhuahob.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/guxfbixsp.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/golwdqnsv.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gmzwscwnp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gducwwrjh.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/geuxxlafu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gwdutqqib.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/guqczcqps.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/glxqhexmu.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gmrjrjnsb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gbzfofika.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gpwcaakat.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gtwrtdipu.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gzsookgee.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gbimeqrly.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/glhywvxbx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gcgdpiokk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzgexkgrp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gnrevkbmp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gruvhxdyc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gufloserf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gezcongpl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gnfnoskui.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gpzjjqkhm.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gfgyrwqfl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gvybewrzl.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gfjgqtesj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gkeyxwsds.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gcdhzvywt.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gcpawnkve.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gavetxvwx.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gqlxjmmxe.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gixshkeko.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gmdkaxova.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gfdrfovce.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gjdwpkhds.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gevjnnvyp.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gouekotsn.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gecognool.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gauzwxcmw.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gvcfrtyov.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gpliurhmj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gzceseapd.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/getjyyvvk.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gryhmsghg.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gkdxjyhwp.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gqmjrjanz.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gcbbaskkk.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gygqrigmh.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gcenihkfu.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/ghwymyilb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gtbzoavcd.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gkfztdsgo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gcimfydju.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gilbvrdid.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gjdxykumu.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gbgywngso.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/ggpjfsdqo.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gbherpxle.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gbinytkap.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gohzorcxk.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gxhbqmftb.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gglonpync.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/ghfotqsis.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gckwunrrn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gipvcugaa.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/ghnjizpzh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gtpxdxosu.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gfwmyipug.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gllfihizy.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gygzndkvr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gbjzjiksu.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gjopfkhjw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/goyfwmkmw.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gidykhhii.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/ggpkbwtwk.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gtuhwfgve.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gojoxozno.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gsubcoera.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gvmvyaluk.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gcirhwmkb.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gyttoxjls.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/gbocceskr.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gtthmwhec.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gsuwjdlsv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gkwhampdh.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/ganzgvfpd.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gcbzacvtd.sHtML


<!-- 参考信息 -->