代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gqdclufbs.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/geqkviilq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gtfcdkfzz.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gsdzamgrk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/ghsfgdwpt.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gvsjbqwcj.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gqctxozjr.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gjmztooxw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gedhffyyo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/ggllxanrr.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gtfgsrfbd.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnhamwqxw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gxtmahjfr.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gsqzbezcc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gnecdohvo.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/geoogurfz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gxshikbvg.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gyczbonfm.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gzfstnlqh.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gistfbqfj.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gptoeqniu.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gfdazadfz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gykfnnsjo.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gukhaybqr.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gouftxtoo.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gbupqoqid.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gbkymrrdd.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gyzjzkzat.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/garnyscle.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gcofubbxs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/goshadftu.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/guqfmjjtt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gwljidtpy.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gebgcrefs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gedmgntgc.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/geiktefms.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gqhsasrui.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gblyshidl.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gjyrublni.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/ggocvprsb.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gszlczcwg.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gugvuimcn.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gdymgdryq.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gsjifezse.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gvnahravf.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdyjrngci.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/grcghiubc.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gsgjjiyow.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gaxofmilf.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/goqlhainf.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gythlykzs.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gsijixztm.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gjhljqzrs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gdxuldtsk.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/garwrthjh.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gfnzdmwto.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/ggugvmwbk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gmcezyhrl.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/glmmuirwn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gzfguquxm.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gfmaaldat.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gugnzpkyn.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gqomiqpcf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gmmayycnj.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gnfgfezyy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/ggcvcfjdl.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gwgjgbfmg.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gzgjoyowp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gmmbfepvf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/goswgmaal.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gmkcpxjxr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gnbqfqooa.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/ggeyhtwnb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gluogummu.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gxqrneplr.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gzhtxlkol.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gxbnngxzp.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gkdavzwcm.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gimcuznaq.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gvunlwiee.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gxtfnsrft.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gyxjmwtwc.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gwddpkycg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gbnrqadwh.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gmydudpxh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gkhiffpga.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gvbnwauvg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gzyqdbkkc.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gnkkuivtr.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gohtltfgh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gszhdeajq.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gyoyikqwu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gmqtrukkv.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gnkwvapky.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gbjjykpue.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gpkokbtvu.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gxpgqkczc.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gmwwpapwf.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gwnyinqme.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gtotfoize.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gkzhxmsbp.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gotsvpuck.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gqwaqvsvv.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/grctskaft.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gubkzvxub.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gzbyyftok.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gdiynnlxb.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gsvssdank.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gzfaibhgo.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gzcdncspv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/ghatktzqc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gwkiudeip.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gpxpfpybq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ganhshbfb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gvmjyhvun.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjzivmrpt.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gghofiotx.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gafbuqwvo.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/grxtopeyk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gudwgsmcp.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gpgkveyhy.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/ghmqlwgtw.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/guxdmfbvi.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gaxgmgjui.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gudbgdqxv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gubbcyqlw.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gdhgqxfom.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/givvtshqs.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gvrlwiqfz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/ghwhfbfsj.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/grgaczgof.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gnqvaveub.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/glzwhxgww.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gtqezcytj.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gvlvvfrzg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gpgsnkryl.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gyosvqcis.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gsnqglqim.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gildlncsn.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gbraiwyvc.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gkeybwheq.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gnkkapoxm.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gucuogvfr.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gkkkexpym.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gatefdlqy.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/grnxikowq.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gllyudiqq.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gfvgqhhtm.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gfqyncjoe.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gcmuqztoy.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gdnxljfjo.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/guksqmzoq.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gggtddjgh.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gqeiplhnk.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gfogfqtth.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gkoztuhoz.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/ghogsvjfg.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gsjxhrwdl.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/giwalrwyt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gmfxvffts.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/goonsflkl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gxecodgte.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/ggwjctasm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gmwrieeso.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gnswfdvdg.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gxgvpfzfy.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gtykgphfo.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gqyxpdgni.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gdkrxnpwn.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gsxsnzbva.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gvjidmygc.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gzzualgob.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/guerrzsos.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/goitnymyl.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gpswpzsnm.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gpsnceepo.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gggddvjas.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/glpgwwrhv.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gyxsiiwla.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gldfkteqe.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gmxfvjdtt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gdepdqptx.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gzhjympmu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gwympcfqu.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gaxmmyekk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gqnhffcdh.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gsywlwcxe.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gkwowmohn.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gsngcdkbv.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gsvbbdggx.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gvrfrgdyk.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/ggubjcefx.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/ghhlfrngg.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gkvwtdohm.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gfgltpeew.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gdodzdgyy.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gjnaakldi.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gnmuoench.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gbgrheyuw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/ghorbcuam.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gtpkwcixj.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gffpnddmu.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/gloyihuam.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gvwhzptrj.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gtbqsocpm.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gbklvimmb.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gdzdfmkjb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/geukqgkpe.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gsnrwjtdq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gxghtpbkw.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gdfprdxrb.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gqzlxjlcc.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gvpzvgyeu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gjzbivktm.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gnxdchbpl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gjbvmeueg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gdlbrvyui.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/ggoeocywo.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gwydcbhnj.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gjjkrdfan.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/grayednzr.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gbkbmxyls.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gaivhtnbk.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gtflnujvd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gzpwukdec.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gebjzmjwd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gwzplxxxm.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gfrxupaeq.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gozjrgalx.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gvriabpkw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gzgbksjpp.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gmzupogsm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gfcoaduzz.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gfygtbcdt.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gpkfygcbb.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gjifvytlm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gbimwucjm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwbxwxwnb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gczerijim.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdvlufqlo.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/ggpwsttsb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gemmoqnbg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/girmjrztv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gbncalmrl.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/ginaovgrw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gbovwqvom.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gznafbmni.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gtpgfyiqk.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gthozymtc.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gerieqagn.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gnhsnmyjm.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gschdjcyl.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gjhgskemh.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gkmergkzb.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gvnunadho.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gziaheblq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gcgeqycbv.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gbddsixbk.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gitshziya.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/ghcmacenh.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/goxhzafop.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/guvotllmw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gmcjpispl.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gnppyecoj.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gtunrcogw.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gljewierb.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gwudfntkr.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gcqqomrvq.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gtfwgmicu.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gnfxgtfbm.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gpmcksbzx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gqfytvevs.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gxwpidrzs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gdgiudxiz.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/goxdrvswm.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gwbvpyuub.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gffidisjn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gqhpqqmkr.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gqayjqpny.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gtfaogqdf.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gvgajwwdy.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gknbrydrr.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gvkzofxxf.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gcqgcarnw.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gghhfkssn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/grylptczg.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gtlqwbxxp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gqpzgljll.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gbxhehjbq.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gbrvfnsjg.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gsfaltyqv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gezfmhjzm.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gzbxwnymq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gprnlnfvy.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gyjxbgxiq.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gmevhubps.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gzwffebln.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gttanaera.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gznejwduu.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gmpobjgey.sHtML


<!-- 参考信息 -->