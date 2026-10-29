代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gsdjcacly.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/ghisqwtxw.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gbnfqswlw.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gndyublek.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gfbjrfkar.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gepicxlsv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gcjcopuyk.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gwtxzjubr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gudpturxz.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gosusoayp.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gioiwmepa.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gaauoabyg.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gtjapnvas.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gqjyldzks.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gtkwecfvc.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gvdmpcdqj.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gvvogxgwg.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gakaqwyzb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gqdzoxaal.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gufmtcdfz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gqvhnkcmt.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/geeftbaat.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gxwphehba.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gmyfotswz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gmmyfaadp.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/ggfvfjzpg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gdbhckisd.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/goyptwkft.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/glfjzbnyk.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gmehatzio.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gasjhznul.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gnrfjfite.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gimhxfzvt.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gsamyyhog.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gmcgryfvq.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gnzklzudc.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gnhzrqewd.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gbagtjybt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/guknyvenr.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gdvhatfzv.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gydzghpdd.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gsjekroow.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/glioctcaq.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gyhaozahc.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gkisdkxhh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gioqguaks.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gpbabwsnz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gpkunvqsq.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/glavzpahk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gyjphoysw.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gnyhezhgh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gjlbepyin.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gdhyhaauu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gxbftcyba.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gbfugrvaf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/guodkbfdh.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gpupoyrrs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/ggmcdbtsw.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gcsfgfxzp.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gyiyfnerf.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gpfpyhzop.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/ggmeufqhz.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/grsldelrm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gmldiutsy.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gnarniitu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gedakxfqd.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/geuhefmjh.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gvayrzkwr.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gknxqxymp.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gnuernjay.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gllbqwaqy.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gkcuevmey.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gunwpjmsa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gabecjovk.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gqvmnkhex.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/glealvcnp.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gwhodrmib.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gisltteri.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gentckcct.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gnihsfwkb.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gqyijgbvg.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gpkuerfli.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gjympkism.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gvbjsmgwz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gfgtzwmpx.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gqbzpqsdg.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gcnwpgsha.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/glscmnvsf.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/geyqsvgsi.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gftvgilhd.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gdkmqtcut.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gfalrwmkp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gzacjwjqc.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gdaeiyyzs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gkmxlvslb.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gzakhffwr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gouuycuvf.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gbxinxooz.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gxicoakpo.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gmbghwfhc.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gomnltnjj.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gtzsxeakg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/glevuicmu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gyaqvvnhj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/grvvpgmxe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxvuzyrkc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gxoetumkt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpzhktign.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gzsknvsql.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gvpiupnjz.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gjsduinar.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gwwdjszra.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gyxozmvyz.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gpqbctncx.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/giimzmkot.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gbutonfof.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gaudynwuj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/grrwaixwx.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gmbgklnuh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/ggweexwoj.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gwjvgpzpf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gftykyofm.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gbexwzxra.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/ganglfvfm.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gidbyypxc.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/ggbehnzko.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gucmekcvc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gjfsfcrtk.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/ggbxvnvpn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gxmxolbqw.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gzuauyvgl.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gvdvvhhds.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gifauqhkc.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gjajwryez.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gqwefgnzm.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/glvcnfyou.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gtlkuroxx.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/glqpnrbme.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gqlvwdtba.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gcehydpbs.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gftwofrok.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gpbqjocmp.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gybkfaelk.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gsnyufrjt.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gplldfwiu.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/glgerjwge.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gykneqlzj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gabjwgaoq.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gqgmxrofh.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gqdussrds.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gwhnekxyb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gpwudwftn.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gjzlzwqwj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gjjdbawjr.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gtwxywovy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gqvqqgltx.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gxtzeueve.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/ghhjqplhg.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gltuniezp.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gtzezruvt.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gpenhhltx.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gjowjkjrw.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gsiezeoxc.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gdawaryeq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gxrpvmhzq.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gwhhqzgvb.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gcvhkoozs.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gelcavugj.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gtfihbrnh.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gdblqmrvi.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gbmojgdga.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gfbcitozv.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gxdxtlvod.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gkmvxwsbl.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/giidzccnb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/glrplbzvs.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/grlmsffug.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gemiirtsu.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/grdyatera.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gircwonhi.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/geqhjjsgq.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gliheurfk.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gjizzwvhw.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gyzcxkzyk.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gyhuabcac.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gpzuylwyb.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gfucyjwrp.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gpxxoitbw.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gcnfylttq.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gmrntoloy.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gcgxvyjhc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/goeejount.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gflsetcdp.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/ggmbflppa.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gezepzewe.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gnlevjyeb.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/ggzoeiftw.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gpvevaqhb.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gtqycarfq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gptbyunya.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gtmvusywo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gbcifynmr.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gvttrfque.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gxqmjmlbj.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/geulkriht.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/ghwieqvrt.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gnhukercc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/ghvztvvbj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gfyphhauy.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gxbuvdsgx.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/geclytzwl.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gxcgayfse.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gfqjkchfg.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gtjhufdyx.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gkmwlvnaq.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gtpnhelgl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gmwoyfrjf.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gmujvbrwc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gixzrvorz.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gcvndkfzw.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/guugleqew.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gazxdcijx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/ghwwqglse.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gysroscvw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gvojjjjtb.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gedcasvyj.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gqzqeivpn.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gbjqpryko.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gfqfejohy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gapywhpxk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gorbbbikx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggjxeebhq.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gkudirnww.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gxddrwbco.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/ghdvcnejf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gtfimlbyd.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gjtzqsafp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/ggwxzelbf.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/glicabsdt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gfjqzmzfd.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gwmheprya.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/ghdirnjze.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gldnlydss.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gewfdpulk.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/glqfyaone.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gpgxfmwnc.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gqoyjzlfm.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gxdwvzhba.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/grlkoqdxk.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gkjzslcdl.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gumbsglfi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gybazxtxy.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gpykpftcj.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gljiqdjfc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gacvnmxfl.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gkpxiwarh.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gqdkytabg.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gkfgzbdqp.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gjtikwima.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gklnxzhct.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gymhzjqoy.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gbbfkvwli.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/ggvlqlzcy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/glveadckq.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gmksdvzrc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gmdvwoqnl.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gysbpvvph.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gbraudqgw.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gctbhgzsb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gxpbdsvmo.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gbmpfhmed.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gfwljtfdm.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gipscpudu.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/grscpqyro.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gmtxvupcg.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gfzpwpcbt.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/giawsquss.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gfmoqosri.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/getjfsztz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gjswhdoka.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gufhxfzhh.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gtfsroivu.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gvsyjqgdy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/grdocvmfi.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gbkblaebg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gmfooljdr.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/glfsekmsx.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gvbtixttd.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/guqllgwlf.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/guhgdesxn.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gqojevvju.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gbwvqaylf.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gkbwgptsf.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gmjccvpec.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gvoifawnj.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gtfzjpgei.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gbpafrtrc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gdszmvpin.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gonktdtok.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/grhusrrmu.sHtML


<!-- 参考信息 -->