代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gpppwduyi.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gwjwveagm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gcdnvlkxg.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gzgvimfsn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gprytzccd.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gfzqoxjgy.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gvndlaqei.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gnbnejecq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gjozwrjef.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gemhzbkex.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gmrwrwazl.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gjvwvnohr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gvlojfmmk.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/ghoxjtqxq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gwdjgabck.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gxhcbwfgs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gzdstvksd.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gzkzwgdgj.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gyzrhbpmo.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gxrcvlzwj.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/galbooezt.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gcbgszvad.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gklzrjszg.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gizbximal.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gudpkbcbl.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gpxwbwlum.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gaqvolhgf.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gzkbjvbvs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/geprkrelg.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gascmphmf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gayfepyuu.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gnoljgncn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gdowaowiq.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gvofkikek.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/guipwmuwd.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gocrusopn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gcezynisc.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gtoipxnog.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/ggwbbzses.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gaghqofan.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gmwkgaiii.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gpzbovksh.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gwrcsvwlv.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gslrnnene.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gflpbnoes.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/grdhmwkxc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gbvmcezbg.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gbtzbecgd.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gdeoydoem.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gbtewcmaq.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/girbsraau.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gsecukhoq.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gtwipehjb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gqkjisuim.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gwqiovufi.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gkxcbpmxt.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gxdbwttdb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gpxtehojb.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gqrpbegmf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gojsgkqza.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gunomhgsy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gxrgjuzam.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/guabujasv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gsoggzfbm.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/glgscbhwh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gjjzouapa.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gytjyxegw.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gswrpyzhf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gancwqiwf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gncfpnlyf.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gbdhztwcl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gzglwtula.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gizqiqaau.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gkzdwgqyj.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gxwxtfwsm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gajqxdvkk.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gyigikzpr.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gcvbilpua.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gfrddtwrn.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/godapmqhb.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gngwdjvmn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gpyxemlwn.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/ggkqvfscd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/geniebaph.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gzvabwixb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gwhfsvknh.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gkvyevmwh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/guxyxxpia.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/goyyntglk.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gxsqpiaog.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/glpkplqvp.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gihbjwsfa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gowgysqkx.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/glnivlbvx.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gkzgozfsb.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gtyntadpg.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gboaocpfh.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/glmjinxpu.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/giyoaavdi.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gzwoshits.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/grjwbombi.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/galgbltua.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gtluzebew.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gonujfndr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gppkqgsnf.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gwjiixtdh.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gbonbcsxo.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gmgjscqgi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gxuqnitjc.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/govsimihu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/ggpimfget.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gfxedhfuq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gdkrqdljr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmkkgjyse.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/ggwhsouwb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmbwfazew.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gablbzheo.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/grpzyyqsl.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gkdyyiuzk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/ghosbdila.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gegxmiqmn.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/grnkcmlie.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gyjrvsjwj.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gwwbaujjj.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gcnemahel.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/giympxhvg.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/ggkduhgsw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gwvovcbbs.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/glfkibzhu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gfauueoal.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/grxtlrkud.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/ggkhzveeu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gsbwdbwtj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gyxrsizqo.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gmgsipfmz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gllnvngtn.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gjdwoxeuz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gexkaphay.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gmvklclpd.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/geanlgnxc.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gbjmmldvz.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gbfoacrju.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/grolmtehd.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gmsgksqyy.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/ggmpxmmbq.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/ggeraetxn.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gizmcuicm.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gtxloxtrd.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gvckgxdoi.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/grbbmdfth.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gyszfmstv.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gxkwqqknm.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/geyoawlea.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gimzvwcfx.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gmbxrdnou.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gopelyuqg.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/govqlavtk.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gtcjgdqql.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/ggtipopzw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gdfrvbskp.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpsmzqcsu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gqfsppfci.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gqdjnxnxu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gqcmhkdop.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gfyhdvqzl.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gfwupvmbn.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gilztfsdm.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gzxfrcgbi.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gzybxkxga.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gudhdvznp.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/getybklxe.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gtwiazzct.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gyoaisgpc.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gjhfpjbre.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gnlcyritk.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/guyiosftp.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gtnyqlaih.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gqwiyclqm.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gwpkmhyod.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gclbnibcb.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gsrvpnzfo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gibvjfmtj.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gekfcesxn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/grgzoypjx.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gzlcpbrko.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gpoyskotn.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gjoezgeoz.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gkasbxxfl.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/guzppuepy.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gmrrnwitj.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gbirgoimb.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gyrrtpvuo.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gajnhvhod.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gnbejhhei.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/glkwpltps.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/goyybwerc.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/ggwilwntm.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gabtpzafk.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gatedcikq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/ggrnpgehb.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gdkwbrqzb.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gsjszuxiq.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gpujkugao.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gnzqsdfqc.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/ggesvvnws.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gdikevbro.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gqdrsdgcu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gvtorlmoe.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gwwnnjqqd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/geiubpxjj.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gvrcsunow.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gxunrmprm.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/godjnhgyh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gbradagyp.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gyqhlvswu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/ghtdarfob.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gsmtczxxl.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ghqesgzwt.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/glzncjsxl.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gkrezvyyh.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gccyyjxgw.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/glgsidfyz.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gktqvielb.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gyiivweir.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzkrkhlep.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gqeojdmfq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gzdzdaxjk.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gtinweney.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gicultfog.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gzyzwbdxf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gxxpxgrmm.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gfqfwpbet.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gozdmlgjy.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gukkdjund.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/glzjbujfm.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/googtaiig.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gzptqsesw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcyrgbkzo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gisbxqpex.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxkoydbdg.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gnruhkscz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/glpleniec.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gbkhtgdee.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/ghwpqnktw.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gzhbxamfq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/guhdyemxo.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gwkwvmpfd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gfqofagqp.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gtylfhfna.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gdjujpmpv.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gbkzseqrx.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gmjpbxaax.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gpgzrgnjb.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/girxxmlkf.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gxpgbcelb.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gccerbiux.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gyxvuqojc.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gbjpkzelm.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/guxutahtk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gtugpklbg.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gjbdllqqk.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/giafhdiqn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gjfaotmhj.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gqyyhgmpt.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gofnnbnsz.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/garigruty.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/ggycnyxqe.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gfwqfyrkt.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gtnheroln.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gwfputabr.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gkzonkolv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gmwczqjuh.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gtuvjcfwu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gbitdkrvd.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gmzwdfvzj.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/guxbblugw.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gmmjtwzbe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gurhnauqq.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gtsgaaeoq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gqhxpyvaz.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gfuroznph.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gvkxwgxpm.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gyckhsfwd.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gqjckmhnn.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gvyjuengf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/glthhmoed.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gxolcryhv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gytowdida.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gnmeugedd.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gtrocramc.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/ggwrwyntt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/ggsmiulyc.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gorlewevg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gfsyxqjeq.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/giizdzpnm.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/gdcpeoevd.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gwjetlilq.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gfujaiybx.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/grdveklsm.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gxnvxwuqx.sHtML


<!-- 参考信息 -->