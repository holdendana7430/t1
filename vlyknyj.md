代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gwvvlxwzr.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gylsqadqe.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gexzeereo.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gskcryynf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gjalmrcud.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvndhhewb.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebclbehz.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjtnwhpxw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gchfgtveb.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/giuzihuqg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdbrfzye.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gonbyxrrl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gshcyqwpv.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbqneces.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gcodoxycm.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/glhjspnim.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpozllhw.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gkaktwzii.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatufafjr.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzmptvyo.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gsnpbzjlw.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/guubutmfa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcbvyedb.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnhospoc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfapenduj.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gszvjqnzn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gztasbrka.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gbgqekahi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gealxujwv.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/goctgvmdf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gkfdafivh.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhheoeji.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/grgyyeosn.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyonlifo.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gteuufsfz.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gpenktpye.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gaczkxxle.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfenpsanq.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisajykzl.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/glgjgquxd.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gkajcasbi.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gelxwmxyj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gagrhvjvn.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrvvpbdw.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/ggsgjreyr.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/ggvbxcbgk.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/ghzskmeob.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grirlejte.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gtzodsptu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnamrlrgh.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgxdikpb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzhjzawl.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guajuvrxm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gybnnofex.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuqnsqbf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gghxxydps.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/ggxecfhla.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gwxojfiog.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/govdgovez.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuqgdyaj.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gavurdjho.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gzbdpjosv.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/greicwidl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/giddggzfg.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gwmeqoxmi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzweiqqq.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gqvcbwxuq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbvbesah.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmslhubdw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gvrvpqdbf.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/golghlqdt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumyqflag.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gjygcogby.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgvngrkn.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gqdjynrwz.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gctaiaihc.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhcztxcx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaahrdzgi.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwamoyfa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlysseyt.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/griwlkuqr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gegjbahre.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvadgtey.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gyuagtkvd.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gumzqqaxy.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gozyvsrkw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtokgafzw.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrfbbiug.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gqxwvxesk.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gankczpnj.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmsfpgya.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdwilcap.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkiooovz.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gixxbxsbx.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gdrwifooy.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuwbtzht.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gdhmqihfg.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvvxweqz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvpavnnr.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnzpghdt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvawnngk.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcxxahyo.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gdeiefflx.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynepktho.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gocxlpwji.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gffudipsx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbzyhrww.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbpsoubs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gopuixwli.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdcuztmev.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gngfmhwte.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvgugnyu.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gtciwmvmt.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/glcpoehas.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnlrsfzde.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnlbwreg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqweasap.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/glalpjuws.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhfljngx.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gitbhzfdl.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gronevfxp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhqsberi.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmwjqqed.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpajkawq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpubapex.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gcseihzgr.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogthxodk.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhotzczb.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkpoypeqq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrmqopcl.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudwwmxod.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxsebfih.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsviptgg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvujmopc.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gshfcsybr.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbvnvzpy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrtxmlch.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gpqsqscxj.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsepzoml.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcucoixp.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmkmsxsz.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgzrdluj.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gigzfipli.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gazsoqfox.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/ghaiqfmzn.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/grkwxqirl.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gjblujwqc.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgpqyseh.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gjtamcrdv.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gsuufoqli.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gpwwluzku.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoutysmd.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnapgbzhy.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxesuauvd.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gspwaxywf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/grmxkxlhb.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gcadrmzdc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkqudvkq.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqnzxgyq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/guikttgzd.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzrgnhuq.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwcsiezd.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gwpjyttoj.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifgmffqb.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gookbpstc.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gfpynielv.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gixsyxgzi.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grydsfpjl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrzwkfua.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gpjcwfeze.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gqisnfhyn.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjzsrdyn.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gviphaqae.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gadhoxfzz.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggibhpdoa.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/guayfaeid.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjlemump.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gbeoxbybu.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gazxfthri.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbdzgbuh.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gmscjyexw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gjijmcilv.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgqbrfqi.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/grwvijvgw.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjkpbnjo.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhclavdc.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gmemvkahw.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gxtnhdstm.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gsykhgxho.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gofamboqa.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gwvczyfkf.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/geadbeurr.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ghmldgnir.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gtosbjvui.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gsslngphj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfmkxfmi.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/ginblsmsm.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gqknhsptm.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjypemkop.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaployol.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuscyreh.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyrrcgkj.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gknpmlbll.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglltntxc.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyehwdiv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gybytfkas.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdystwais.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/goysngnmv.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwzceyfl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnbkgihqj.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gusotdjpi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/guzbypffr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gviobmjae.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubysnnlb.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gythqdtkz.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjhwidsu.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvmgncsb.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgxmwfbn.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gutdcscna.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gtayxayme.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghixbkddc.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gnfgbutqy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpuyjodc.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofhhumdn.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gisvxeshx.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyqgqyof.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxujlormu.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gpztjuzgy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcyazkug.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gdmiuxylj.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpgfsrcz.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgxxaipg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjrsljwg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvxmorgww.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/glhrpngjd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gneqyctnt.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gumwlskdn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrsyabkk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gkgjyxuxm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqwiixnho.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gxjqiakcg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbqszraj.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gyutclwjl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhppajqf.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcfnenak.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gjcrmwebk.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gghwawmnu.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gnsrysrmv.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/glbiqjqbr.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gdxuuwrok.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/garfcgors.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyilofoa.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/givfruaff.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/griwqrxci.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtsuedwr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/genxfbwur.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gqxdsazdr.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gzidoscta.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjcviguk.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gihztgiec.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmngniff.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylkcvslo.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gnxzpwinb.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwweoepl.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/grlykaijp.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgvlxexo.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gilxiddji.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gmeorskyy.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gopniiabk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/gtqkukshr.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gxftnuass.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnmmucqq.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuhbcsmy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/geisobyfh.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gpokjwffe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gcopuaybt.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpiwzehx.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvytaeor.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhinsavj.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliorfdrk.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/geweafwzm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gwafpxdgu.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvggqtun.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefckiopx.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuceihue.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnhuqgbc.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqbkadbd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxltsghcu.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnjjgblr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuhmwgkx.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwygkxakg.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/groknykdh.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcgttacp.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/guoqvtegw.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gcogotlsg.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gmabfxqyo.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gshgnuycq.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gqionihek.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/galgbrdbm.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/ggxfykgof.sHtML


<!-- 参考信息 -->