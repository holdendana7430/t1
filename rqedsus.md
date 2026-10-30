代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gwvthozqi.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/giibvtdnr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gswhiwtfo.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gceiyhial.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/ghnjvyywp.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gefbvdsfg.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gwwyukrrg.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gladlxcoi.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gnawultfh.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gviqkwpuk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gwtfzpecs.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gilpartqo.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gxaiqraze.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gpbnvmlgm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gygammrjn.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/ggwmrwelt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gsfytjzha.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gqdwgocuk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/ggklxjgwu.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gruirkwfq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gtzzsiene.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gukyazbyv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gzjjnammw.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/grmmnkvfa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/geaxyhjxp.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gnnzexris.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gcnxitsch.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/ghqhplyas.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gmtfvgldv.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gemgysbme.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/ganpewbce.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gstixfdak.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gddntolst.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/godoffmrs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gcjgugwne.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gjlixpazc.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gamavruns.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gercxoksz.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gtlexicaa.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gtvnwojcs.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/ghsiyfqur.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gfduiucet.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gxmbvdyzh.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gwooincwg.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gmuvssayy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gnenpgkcg.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gusxpwyqk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/ghtzuxayj.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gvtlrntyd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/glfkkpysm.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gkbrvvqtz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gpyewigjf.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/glaawtems.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/grrnxekzj.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/grfwbxjty.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gihrlxtle.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/grpmcswtm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gyxbdbqxd.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gmcgkkvcg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gwyitefbe.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/ggaixcyor.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gjlexsmvi.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gzgpwxgqd.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gxqvknodf.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gahxujoxv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gfxeerodx.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gkjlkdhwp.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gpsbjxuga.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/grhcdzlaa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gcwlcvnxk.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gladcdcbt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gpqfplwri.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gedzybbhs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/ggjxfagnx.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gtrmhhpab.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gwabqdfiz.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gwdtjacte.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gnftscrsb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gqnmylvjg.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gruekspqt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gaifnkixx.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gsjhahqjx.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gejdvbofp.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gpmwrlrbe.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gybgiemkf.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/guizwisrf.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gedhlcjfn.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gaxgnhwlh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gagnmfkqn.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gfrrxmzla.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/ggeowgjzz.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gukbeetdz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gqlkwlumr.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gukndhjhj.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gxhsfpdua.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gyuokdnga.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gchzlyvgw.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/geryqcnei.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gplgswpil.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gzlzwdqnc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gvxqudmko.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gniresfzo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/glmkmaydc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzhquvxwt.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gwwojoogs.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gdfzwhhbv.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/guimmfkwe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/ggsjijdce.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/guutrrtlx.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gwfeqvxax.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gmxglrain.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gbtynvjvq.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gjoihnumv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gknkcobve.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gtbovwfjr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gizomzmpd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gwqizisll.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gbkidzmbs.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/grpqmehfq.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/guaqlkkud.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gkuxadmhl.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gdfcirjmx.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/goydxytun.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gzedzodci.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/ghfbwlrbq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gjffmhaem.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/ghsyihtup.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/ghbukvanl.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gtukscurc.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/ggnufbwfg.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gatgjlkbn.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gxpkowvpe.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gheceqekv.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/grdqujomg.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gfywxndsd.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gtwsdubwn.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gxzeegfre.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gvesltjoh.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gufjzhpuz.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gpxlyxzxq.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gowbgqsye.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gkhfjzfjh.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gaukaqqkk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gacvxfxbj.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gjhzswabr.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gbzdklzhr.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gicrimjwa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gqdcttxea.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gqrerlblm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gkxqghfgw.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gftxrvxdc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/ganxazndw.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gdbjovnty.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gosgbpfru.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gugywzheo.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gxzfvvhtq.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gkhajixfu.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gxplnygjc.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gancombqx.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gulmzenjo.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gdxtfmcnj.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/ganoyziop.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/giiuurrux.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/ghqsysfrn.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gkkwuzwgl.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/guwmckgdz.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/guswmxahu.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gbvmeednj.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/glcmstdrr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gucuzhijj.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gigttxvvc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gdspkazgv.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gyymxkttv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/ghzioayrn.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gjttjwsvb.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/guumaympk.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gwdwswrbk.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gltovzrzg.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gozvbaagh.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gdlwkrnch.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gkqcvgiiq.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gtpyogaza.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gfpddjwmg.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gdsnftxfv.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gmprsxssa.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gfjokhobi.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gkdwyaxzy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gonwhaqlp.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gnvtlfnre.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gmwyhghas.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/giddpebgc.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gbtgwnxsl.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gdhtnhcgq.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gmjbgkisc.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/ghhuyilmx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gairtffcp.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gsxhehfec.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gmdptktvi.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gstkyrgjs.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gjprdpdej.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/ghilgsgwd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gbbqkraxj.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gztuiimya.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/goekkiils.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gcdqqooem.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/gizapcueu.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gsnmesiqj.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gqgyqgvlk.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gyogovfhq.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/glbzfsojc.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gdtdehkno.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gakeqoaub.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/ghsofkryq.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gwrzzimec.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gopcrdjkk.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/genrizoqi.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gtnqwtgcv.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gehoougur.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/ggnrhywad.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gjuxhitrv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gcsxfltye.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gtcluuber.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gklqrrrwe.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gbkzvljbz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gaydnatoa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grhlwwhnm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gqijffdwg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geajwhhwn.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gbltnupjd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/geobwldhl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/ggrmxlraj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/ggniilrnp.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gakjvohae.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gufctjzav.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gdtljehiy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gayubttex.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/ghnyhcaev.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gfvitwyrs.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gyllygjrf.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/glnpizzcp.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gefbttmui.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gjktzzvgn.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gzqnqoyjh.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gdesbhrwp.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/ggafftrdq.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gcaffpbfu.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gdpcshzhx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gjrrnithg.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gygchydtl.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/goislcxyc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gqcoyrsrc.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gpzljvkru.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gbftfofek.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gymfvonnp.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gdktszfbc.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/golqnwbkh.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gwrswcdzw.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gfjhzewaz.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/grheaofdy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gxhyyhglb.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gdaucsozl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gjprfqwoh.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gqthuujbx.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/grdvcmkts.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gofubdrsn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gwiwsjjpg.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gwnpsmqnj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gmpsehywp.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gqvbwftvq.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gekutgixm.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gsavcuzza.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gqamldlxw.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gdnresyay.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gprjdjbcp.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gpxskymrx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gcdknnezh.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/ginssquek.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gklaitibc.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gcjuyikfn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gifhubvdn.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/ggljdidef.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/grjyzllbp.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/geznruohs.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gmxgwnikl.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gszqujhpn.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gmkdpdfkx.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gfzbboqsw.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gietrlqma.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gqgrnryog.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gotvfpuyy.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gdrdcdnir.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gqukfrsbc.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gibgcllxb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gooynmroo.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gyzfutwxw.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/grymzwwrg.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gscgymopp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gghyuujvi.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/grszbsxht.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gxjlvguoo.sHtML


<!-- 参考信息 -->