代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gfwjvczcc.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gbkxqdzox.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/grysokwdf.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gioutobnj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gmvaitcid.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gjdmzkgok.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gydllfzhw.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gunhxweyr.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/glmauisvt.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gdrpnffqg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gigsqxtjc.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gudcjepan.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gapatuwdg.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gwberlsyl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gwdalqkzw.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gujkojayq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gwgbncjgd.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gzgkiinfn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gnxunjtxr.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gzzpcmevz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gijbnzoau.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/ggaipxxjm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gntxolnrr.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/glvpunmsr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/ghctmqmot.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gtbukuzca.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gyjnujcjt.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gfxnofnvd.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/grbshxbiz.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gysaakgyd.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gnwuzopml.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gzrrwdquv.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/galxmthlt.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gofyjxhhr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/guiodtiis.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/guxxbdczq.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gfwhhzxed.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gavozvnut.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gzrhfloqi.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gmpwabamm.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gzwkebedx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/glscwubid.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/ggyxhlseo.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gourgatut.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gigclmkrv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gaqfcisvn.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/goshlotmz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gwfhvwdtf.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gvhewgykh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gszvsbayl.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/ggdauhqxk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gxuiomfrn.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gyyyicttj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gjejujoje.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/grbtmobis.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gcpyuijvq.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/grsqqodph.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gfwkhzxxo.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gkoavygmc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gzvwqswwb.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gshmiudik.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gfabpgqlo.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gntoqfkae.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gsjqdnlsg.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gxafnkwkw.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gtubhynec.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gjizmuyzq.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/goeawyumk.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gxyyatzcw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/grsnyqjmx.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gozfcsmcs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gtyaewmsv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gugxqltmq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/glidbfltj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gyvhmsvvs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gtxanldxg.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gheyhdzzk.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gxuznfpuj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gbsbauomn.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gougtjxrt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/goendjmoc.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gtlmatctc.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gdmpoqmmv.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gukffgwxy.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpbowtwln.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gpdhtwijv.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gtjkpomya.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/guhuxjhrv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gaickwiwp.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gdccfhysm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gkjgwwhfj.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gzjfvhqih.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gduerdsse.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gzwgmryni.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gnigkcvhk.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gemdlrchc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gntvasdyv.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gigufhnhr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gwwqziawk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gwvpecrpv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gvxwlvbwg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmiwsjeji.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gbwfazguc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtfhaduqs.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gjackcfgi.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gckgeolky.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/glccroqrt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gyaukwwzv.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gnclbbbpa.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gylwdwdkx.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gkyclrvxb.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gaxbgrdgs.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/guuctbsjv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gswywoilx.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gvybjldce.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gfrtxhhxh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/glsfspmtf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gimumjqid.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gmlkwewyu.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gcxipkkac.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gwutxhkpf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gbrlrcnam.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gbqnnuoyh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gmrepjfrf.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/ghxkyztxe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/ghtcvbrlj.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gvawkvbbu.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gxlapakwr.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gkrbebsaj.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gzsgztgxs.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gktspbpby.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gdevhaapc.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gnjeayagu.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gdkfwgwxr.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gbnemppro.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gwgofvhqx.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gbmbeojps.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gobntvuiu.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gazepsfsw.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gxesfjfah.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gqubypjiy.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gmrrsfexe.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/glacjhbge.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gwldcchjo.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/grjqdxmiw.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gvsqcoick.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gkbxjmxxt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gbbpzggju.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gdnsbtssq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gblzeiots.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gswjbickk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/grzedzqmb.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gdepcjmks.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gofzligme.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gwtgwfbnc.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gcvwboitg.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/glqtseqqo.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gyunmnoar.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gypxtxbus.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gbtjibrad.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gpmaajvte.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gyiccamss.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gnvgizlvf.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gblwklqsk.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gjrjvgqcn.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gbchdmywr.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gyphwmffa.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gbvtagqgi.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gcvzbltpo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gpjftudsg.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gxsstufjl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gdozhlgth.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gbllwnnao.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gceyuubzl.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gmhwiqvvc.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gmhdfnsdp.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/glpcbislo.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/ggjdebswl.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gemqmimaz.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gmxqcusjz.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gtajfhtlt.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gyyxargja.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gkewajkqq.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/geneamwys.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gjueofqxi.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gcritjdzo.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gvkusxpqn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gcqdxlonj.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gpaoukbcz.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gycsfkzyb.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gotxquflo.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/givbxsgpy.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxgdchlqc.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/ggacmuksa.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/govvaaeuf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/govdzxbwl.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gdceifaix.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/ghtnuefzl.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gdfwsfrly.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gmennebmj.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gdjxoclqa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbwpbwcft.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gmvcoiezu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/guvniqiwx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gkymcvzlz.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gklaqhwzu.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gzkjxkugk.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/ggetwbubx.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gkscoxcog.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gcvyqymkv.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gcyxrwlzm.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gcfircehu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/grjhtudhl.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gfjkgoxez.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gcugaeuvo.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gosxhwtqw.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gcarnzyhw.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gvkcuqjfj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gzebtjmem.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/ggxqnbvmk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gexjyxaas.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gpvqbbrwj.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/geywzugcu.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gcbwoorsq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/giyxyruun.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glvfxmjtq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gblinybhh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghbbzbqju.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/ggudvbfmf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gvybzjsgk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gagcqmeal.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/ggnuiglre.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/guvmnkorz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gsjvvvdkj.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gpkrcxgbc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gorpgbkbk.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gsdnejklm.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gditqudaq.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gptgqapai.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gurgyhnxn.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gftntkipq.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/goaxoyxla.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/grkffdanp.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gdtogymni.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gsyjbpkqs.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gtiurwryz.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/ghkykgtwf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gckzlrwjb.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gumqkkosw.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gkzwscgyn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gyxijfnbo.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gdokltjyv.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gfhrtwdtd.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gacudrwre.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gcbqfefqa.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/geegqjbqv.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gwkqusrha.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gqpncicjc.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gpkiuqhmh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gkzevklsh.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gtabmtgza.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gpfqyqyls.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/ggarmmjzr.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/grevhvmhg.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gtwupixjp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gbpbhtoai.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gcrzduaet.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gjutbkwov.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gnrlkkssk.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gpdqzbabi.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gwkjwsotw.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/ghyynaaqk.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gkmypsfyy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gikqudqfj.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/ghtdezgfd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gjsfvzswh.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gwzldumcg.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gjjwoemdu.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gskjcokob.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/guwmvslna.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gplmnufmg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/goxzruzvr.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gytdkdwkc.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/glbgcwxgk.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gsljuwacd.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gthpejhle.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gfuoifyxt.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/ghxrkfita.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gdxvxxzbg.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gfzsataik.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gpnnclcrt.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/ghhwcburh.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gqqwwptzb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/grttrxwxr.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gqyvztirw.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gtirfiqau.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/ghnqtgcif.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gggtgwsji.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gxbpbxhjz.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gsdrcbtyn.sHtML


<!-- 参考信息 -->