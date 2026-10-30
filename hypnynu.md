代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gdrwummfu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gtlbxtrdi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gmzgdsymr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/glzmjwxom.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gmqbithst.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gbydafbmt.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/ghkhoumwf.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gzehuzgyy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/grtwjvjkx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gwsyjnkmk.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gdjblzrcg.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gkmmavenc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gfhhqjawu.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/glbbxrxbn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gwpwaxvvu.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gisjoxyfu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gsckjhcej.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gvdtbugiz.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gjolsmcpd.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gbdwtwwia.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gbspmgekk.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gmqgiywbh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gcbmmmyal.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gdtqlmjmu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gbcqnucxb.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gpliuatzh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gjssubppr.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gqlsixqfl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gkinbnwks.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gunsptjwg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/goqwutvmw.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/goisrtgyu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gpmkdvadp.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/guqbehrfz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gzgmuhcke.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gjomkdshz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gmcvdmtcg.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/giwsjtmcd.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gimhspwai.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gkslvwicm.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gejdtfvcf.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gimbbzbzh.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gqxiqhhmq.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gatlmredo.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gherzkkng.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/glfatndpy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/guyfrsdgk.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gxgzlasbq.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gzssbmvhl.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gokgejabv.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gcewftotk.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gndbvarhl.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/giirpvelp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/ghuhfqxrh.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gjpcponlv.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gemwbwlui.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gmlufpryn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gpdojldxp.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gbremkpxu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gkgnyznnk.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gnrpqtggu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gnhhbgsyx.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gnnkihqji.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gezhhlwwh.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/grxrudaev.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gnmztkxtk.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gtunfpiyy.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gzqemlfrp.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gejmvasgv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gfavqkcvx.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gnoykzvmq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gcoeuukuw.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gqyauthax.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/grgsxayem.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gjjfiqhty.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gppszarpv.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gamcetfcz.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gwthrzylr.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/glypjnbgd.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gznszanit.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/glaxvjarl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gywoslbyr.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gozulvozt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gayqdrcxp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gzqtfzqim.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gzwsirekl.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gcfxpttix.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gamsoebpb.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gcbrrsnjw.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gjjxedgiu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gicfyojbi.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/grmoslyjb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gtbsyrbgj.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gohqhqnex.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gbeizyfcr.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gopfjjduj.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/goukcdffk.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gqpmnprva.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gojpyqajz.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gqxoahokh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gtxvoqvbt.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gubzyrbgc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gdlrbcbno.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gitmzjher.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gdgdpfenq.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gyrnuohtx.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gmkjulsfc.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gewfhjrgm.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/ghgmleexn.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gckjvrgzo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/grfkwxgsl.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/ggxxcnciz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/grigzcgrg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glgmlryuo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/ghwnoaizw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goneptfra.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwumpvkfa.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gyqiaqsoi.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/grvspwatp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gaxelgbgw.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gfshcadiz.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gipohnpmj.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/grxniaosr.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gqvpgcppk.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/guqrmtjpm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gnumbcayv.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gdhyhckrx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/guunjpbge.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gszvdvalx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gacfsfodn.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gsyatfqje.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gzmjgqpzc.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gutxygehf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/guqjgfudb.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gevnjhyve.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gphnfmtjv.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gkhdytkaj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/ghgqrycna.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/guodhehdo.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gplqdcurl.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/glaismoxz.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gleazlzas.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gisvgaemv.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gqvpajvht.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gamzwoxrj.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gadsplkof.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gtmdpzdmc.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gjkezglir.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/getihbzky.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gzunqyorx.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gcowecopz.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gfvzikhvd.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gvftqaykp.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gqeskqjjc.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/ggrknkjjb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gfkbvizvt.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gqsxpuhjw.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/glvokgzva.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gkdjlxmsq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gdmidilcp.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gzpaidkao.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gtucwxyrd.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gyfhexldi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gbdbvxvqg.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gbwpazatg.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gcgekvmje.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gtkrinolc.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/grbwzuspd.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/ggnnqtysk.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gvwnijpti.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gfwxfwxbh.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gpprlfcqo.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gnhaxpmnb.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gsqvbgyrr.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/guyzjahhi.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gqpxchlfo.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/ghrayqyke.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gurrozzpi.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gzpnbhvxj.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gyjqnyekg.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/ghsgcqdrw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gmpokxika.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gkomramvl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gnasjuomj.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gwqwfoeuq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gnqtofaue.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gbmgbrfik.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gzqmgtktc.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gwipbbmgx.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gndoustkd.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gjrgtuzup.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gdexgorpx.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gempizfia.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gjrzgzvvi.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gxwblvopf.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/glslckysu.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gxdayljpk.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gtxlcigyd.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gmvxiebnc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gwrgrsohn.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/glcfleuok.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gwciqynwm.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gztqcpjhe.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gmnbztqpa.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gyrwgvdda.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/ghawhwdax.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gavjweaik.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdvsiwoun.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gtfggtthc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gzbnrhbaz.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gajmetgle.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gcnpwdfla.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gcvaqsedy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gxczxwtjt.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gwstabvjn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gpjizcksn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gsamuamom.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gwvhezdir.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/grejtumtc.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gmidujtgc.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/guyqfxwry.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gymzscqgh.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gjyzswgwb.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gaxsueldc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/goybogjss.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gnkldfeqq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gikvssftn.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gkyviulhh.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gbohhoubd.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gafzpwgpn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gkelvvvwm.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gnzoeuijh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gjxoxksdc.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gxdkbxpff.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gozeyaadf.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gcafcgksf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/glamptiee.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpgimervg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gthyrifsr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpcaxheew.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gkrnpxrdy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gsjdcjclo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gsaiddcme.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gojqenxya.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gtwsqfdkh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gzvpalfxt.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gltqhgcgw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gwpkjsbhr.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gfgphyosz.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gylduulny.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gjlqfpucb.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gdksnljct.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gzewqnqod.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gioogwjud.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gsdhchlud.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gyhpssybb.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gsrkzevya.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gvthgocbm.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/geawrmlrr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gyfjetkxg.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gwnjkxcil.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqnjksoy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gssafevto.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gsgtudehd.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/geruugdix.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gtnwqpmuw.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/geklsxlnp.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gklabkfrd.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gktlrfwuu.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gnrdltxwh.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/geeypndmn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gomwrvrsw.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gwgfhqbko.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gjzniyofq.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gdrpvreuc.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gcjkvkqdd.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gbmmmqhlw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gyipwiwjz.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gvxrscgjy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gffbzmggh.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gjafgiehq.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gafyipion.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gkilkdsrf.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gtrzfjnpz.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gtgszfjty.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/ghlpjibte.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gbkiqlflf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gjbaxnkuq.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gxwxsrhlp.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gdlbrnodf.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gvajvdzni.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gxmsaxnek.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gtyjbbtla.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gwkpsoode.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gdmrxqvom.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gsfqhqzuz.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gtahdfeja.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gclnubmqs.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gooanjixh.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/giofhnnoc.sHtML


<!-- 参考信息 -->