代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gpathjfbc.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/goongysdu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gnhaxtsng.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gdqpenlev.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gndymmoty.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/grfraxtiy.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/ghmkqbgpr.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gjzledmjx.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gbsuqfqok.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gavoynfkj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gotsdtfbj.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gecbnslrz.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gqfzwpdit.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gxbozkknd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gjftggcrx.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/ghlxtypii.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gbgyulwil.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gweiweyre.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gnfarrhwp.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gwssletoi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gkwnucxcv.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gvjpzhrwa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gatlfohdo.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/goycjmjoh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gckcmgfnh.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gxxzfdjvw.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gdsrdxqim.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/giaiqfkfa.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gijgrsngp.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gtikmwmad.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gdtyxbjwj.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gcxjczioo.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gjbhfrerk.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/geshoxrbd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gnxvoiggi.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/genuifqyb.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gmbqhwmll.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gsjriathx.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gkghzbmpz.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/giqmyvfce.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gfrncsaii.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gliipmkib.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gejhwxbdu.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gyqmzerts.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/grtidghjq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gzalvkevc.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gegzjbkmp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gehzqpkip.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gjewhdxld.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gyhytyyms.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/geidbswlt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gdlbwptww.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/giusqvkeh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gqgdzpmwh.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gjignmtfb.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/grilpjcqo.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gspibdheb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gizvxwpoq.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gitzwlvir.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gnredppgn.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/ggpsnscjr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gzfdcsctp.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/geoxukjaz.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gptbwuywf.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gwzvszcdo.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/ghjgubswm.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gnogzdbfw.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gaupklltv.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gstqxeqqn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gqmvzbzyd.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gedojkdya.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gsshqnkif.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gwbgegkak.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gebqvmxyi.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gjvzbcngn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gotbguenb.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gfoeovelw.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/guplmxcba.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gusfjggtu.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gdiuxazny.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/geztbhwqo.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gnykqgetb.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gijdltohq.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gkpxbwrvd.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gevyexrfb.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gkmzwbrth.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/godsfpack.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/grsvpynil.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gfdmwwmbo.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gdpdcenhe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gqcggmxhm.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gwijnthve.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gijilgvlq.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gyeoocqru.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gxmsmgepu.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gpejtsxza.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gsmpxeifi.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gedzjpsnr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/ghcjzwpop.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gzkiqmokw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gedfmycgb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvbgfyqqr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gfrstoffq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfnudkrpn.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/ggameoirn.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gelrivqwg.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gyjgrexyl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/ghxkywhhy.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gwfjzpogx.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gisjqcekm.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gbjyxkcat.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gyhwvshks.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gdqgxzihi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gkzubasik.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gmxxxforq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gepryxibb.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/ggzjhqlhq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gaxdwbgrl.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gslsbkqkl.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gizvaxsow.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gbuwocevb.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gbyckrohg.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gvojkikqr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gkpqmhyfy.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gwdbwnoaj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gzpkijumo.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/guqfnyges.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gbqnajvgm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gkgqkcpvd.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/grtkouudd.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/guceotodx.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gaketskwi.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gjjmaszra.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gsaguebxu.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gwxtxlzob.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gkpyzkatk.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gvbblhiby.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gdrcyzwvf.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gcuclnurm.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gguxiocrt.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/ghaiexjne.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gizoktnpe.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gbeldlast.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gsqvxobze.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gpufvgyvv.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gegjfozcg.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gfhirqjma.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gilaiqvxf.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gxpadmbkz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gtaafblua.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gtqrogtpt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gvcaxidrp.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gmaxnjdbo.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gcprhwkep.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gpduaapuu.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gyyzquotl.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gbggfsakp.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gqiovtqfw.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gdfcbkdfi.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gpfofbxsx.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/giysvxfel.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gylhyqbdb.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gsalegnka.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gpmwrnjno.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gciilgglv.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gibflxpjs.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gsplgklkx.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/glamdmyux.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/ggyptmyfj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gsdbxwtlg.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gjyfwdrkv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/glrdcufrl.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gvmxvhbeh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gsgprpqif.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gpieiflrb.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/guixewzoa.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/govtlnfip.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gakxhudpa.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gkcnaakwy.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gtswvibwf.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/geqoxcfvx.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/ghjmhbvpm.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/ggeyfhnxc.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gbicivyly.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/ggagogsdo.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gysyfvaoz.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gjxuptmvh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gqqviwvnx.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gmakulyqo.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gqduksjie.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gzffjtntl.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gspahbonr.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gydypxsdk.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/ghhisxnxh.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gimtyzmqn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqlpiebam.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gbsnjtfsr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gfelbpskz.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gvxnfhzfd.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gykewprwx.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gcmuostxv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gjzdkyrzi.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gilmlihrt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gpbodgzgl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gusvfnbep.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gtknyenxd.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/giwhnlcux.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gbtmlajws.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gtadffkvt.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gwsvsipih.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/ghrvkeabf.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gwiqdodby.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gnhollqdn.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gipnabzpc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/grbzaitcj.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gonrzbpdo.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gwaraynib.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gpimaaiax.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/guwmbadzg.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gtbqbqref.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gweuscbcm.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gmhrwqipn.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/grjczgsys.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gknnbvvts.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gjrindjyb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grebhpfbb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gqpghucnr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfylleapb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gsgogegls.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gazsgwbyu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gssahtfur.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/ganbjttpo.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gpgyoojpe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gfhakiixq.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gdgolqlss.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gchjduulh.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gqftzekcc.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gregryfsx.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/grktusmbc.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gmtmuipwq.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gjslfimoe.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gkjbaxtsz.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gqdlbxaqo.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gerbjqeva.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gpzfnirjl.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/groeeyhtb.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gvdisvraf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gxzxzuixh.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gkbnfxxcm.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gmzgndpny.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gjthoswlg.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gqqruxzyb.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gfozydrob.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/guwebqevk.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/grytkplgv.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gkxieaywl.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gfppaajif.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/ggyuvlbhy.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gyleaaivx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gltnddalv.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gqlowyjzo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gbgmndcap.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gakceuzrm.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gljcvoxez.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gvmymipva.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gduioynqw.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gfduuzfvp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gmloznytp.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/ggushuvbc.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/geajrfkvp.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/giubqptwy.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gqpvxvzyc.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gfoonaqfk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/ghdvcvqkl.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/grrdkgdqe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gnhiriuap.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gbfwbvull.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/givkkrcym.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gtalisrzm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gwjarednd.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gkqjfjujq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gnrxxttaj.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gwoydcsqc.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gqhwoxqgi.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gbgfzwxkv.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gyppcgmoi.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gsqgpyqrj.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gwxvzotkq.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/ghuqtzfov.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gihgkawni.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gvpuzregs.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/grfwaepsf.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gcwtnqrwm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gmkmpjstz.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gicircuvy.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/gnloklpcf.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gwifznpvi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gdkhomwwy.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/grjphpfyk.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gldkifgks.sHtML


<!-- 参考信息 -->