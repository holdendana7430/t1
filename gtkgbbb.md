代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gyrwxkwxu.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gedmgouye.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/giwdkemqn.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gszcdsxdr.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gatzqfeik.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gajisxyvy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gxgsrrpua.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gynwbjkss.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gydxmareg.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gknlnusqp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gkicvauxt.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/geryeckol.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gyaqoosud.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gqbycdxub.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/geqhbmpcx.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gtsvsylve.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/ghrlsixuw.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gqzoswwsb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gbrzqevgy.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gcvsoaolq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/grvshtxgh.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gelnotxln.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gohbizmep.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gdnffweqy.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gzwlnqyav.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gvzefmqvu.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gsvcjaqov.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gbvpslqnf.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/guvhtjwvs.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/geszrkcyq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/glccuhjoc.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gbflpkmaf.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gusiqpwxn.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gwypxnhdb.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gtrngyjvn.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gyliugldh.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gxgbcwxhp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gtwonbmyq.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gwsrkdckf.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gaqryluvi.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gnwspwycx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gzlkzfdrd.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gadxcqfue.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gqazgsmfi.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gdnrowcep.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gbmlxbbas.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gkwmfjxvp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/ghrcymgtb.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gvjhnpynq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gkeqstwwm.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gpawrlaak.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gbzwjvaun.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gjyloklbi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gqvdrqfbs.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gklpmdoup.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gfmghswkw.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gsmywinpx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gwrhwpzfs.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gzoyqrqpu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/grjpovtuo.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gvtiylyny.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/guozlcqws.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/geiqhpcuf.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gbqzgmtjq.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gutpwqsqa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/ggjhududa.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gthujjkmc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gbmhxyauz.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/glgzwsiqf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gqtuhtxnh.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/glgfrvtpf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gfzyllqan.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/greifcpvj.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gzgowicds.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gncacpzzb.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gorrfpmue.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gwtkverht.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gaxihxrul.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/guxnobtos.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gatkylqiq.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gjezehsel.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gotqonrms.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gepxpcpjj.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gbjloblgj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gieufwsvn.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gsobgztwt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/groqfslfi.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/giocaetpv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gdpriwbdd.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gloklcfyt.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/ggwdvqlvq.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gdafjqlzx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gsgqhaelb.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/giwvtkvig.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gmfiegasb.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gyhqljjow.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gzchtmtke.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzauxymuf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/giskmlpwx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghdedtngh.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gpfyfgucn.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gaddlubha.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/ghvplrnwm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gopdxzrle.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gjybdzvlt.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gnforxlsm.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gwtrkeqnw.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gmzrnxhgh.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gqejcndle.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gvhmmbzpa.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/ghswqzkth.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/grsoikoww.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gtgbqeaux.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gyrycglsp.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gbtujccxp.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/ggywgtggi.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gyqwrvrxe.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gnrcollus.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gkkdidzmd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gdixgifox.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gyhjhsdyb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/glhzcrcho.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/ggrzkjfps.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gpgvfguzw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gvvwwklyl.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gwvbjjcvg.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gnbxfpkgw.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gzwzadfzp.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gtxigfrvw.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/ggjvkbdab.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gidxtivxr.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/glxpmyypo.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gdumbefyx.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gigidujka.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gamtoprkl.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gbeuazakj.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gegnnenru.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gvslhfdwd.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gskuqgtnu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/ghnfyactv.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gylpqktwk.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gvoejqxzw.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gqurbodah.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gpbkpdugg.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gjuhaines.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gustlronp.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gsmuxictm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gymomeedj.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gwdnbpwde.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gifjrinve.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gxhvhlxia.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gcnyycxdt.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/ghzxlykio.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gdwmgbusf.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gqmtoupre.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gwemyymzy.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/goyogjcsv.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gqwetcjbo.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gpuqivuix.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gpeeqcvvf.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gdkhwsnwd.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/ggpuegihb.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gflbuealz.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/ghxpsqtse.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gawhujzuk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/ghjrhpvzl.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gnlucniqf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gvbbwaggy.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/ggcqokofr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gyqjuegie.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/ggvdnfjsq.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gtwumdltj.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/glsqndukw.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/goqovbenl.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gwwmzmkyb.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/geomkcedl.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/ggbhppxas.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/guqzusvhr.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gjzivqxuq.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gewsmeetu.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gwulkzulo.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gaburanwc.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gtakliuvk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gtygedjfz.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gdxbzlxwr.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gtmkrvjko.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gqtekkycm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gbibryatw.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gvicljzoe.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gwbifnlrs.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/giniafvht.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gnalonaxh.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/guwckseaf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gekaglyue.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gqcjyjqjo.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/grvxbcggp.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/giuxghkcd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzuwnnwwb.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/grqkxxppo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/ghivmqqbb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gdghdvqbk.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/glfjrxfik.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gzcwpcjek.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gfiyuaaem.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gdirounpx.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gkkcfxlqp.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gysfzlmwz.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/glifsjvra.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gfkxrnnjx.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gzgniyvrn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gtmrvomfl.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gjraewpyc.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gehutckqp.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gnnqtznpa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gciwxkhaf.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gljpwsdlg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/galpiohcv.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gxkghmfwp.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gxrxrdrmi.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/grdmimczk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/glyyviyad.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtbfhbyut.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gznehlriy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxbgzxxxk.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/ggzttxolw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gyoqkaokw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gulnqxfzz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gskekhgte.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gfyejvrur.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gsheyiaev.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gfkcevdmm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gyelialwg.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gylshdxfo.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gprnfmwau.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gkiydzzgm.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gejezywwi.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gyhmldhjj.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gkuedwsjz.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gdcxloxls.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/glsxadsde.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gdagplnff.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/ghrxukvwt.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gaihmcgkr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gqzzpbmve.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gtgdegynp.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gravnqrge.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gxxwcakpz.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/glfwqxwfq.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gyrqxftfj.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gaaimwrwb.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/grdpplngs.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gazpvcnof.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gxosmfyfd.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gmqiqlmuq.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gxsefsxgm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gqbxhcbho.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gyvcmxblw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/grtdlwibe.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/ggwhpzdzi.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/ggxxagjjl.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/glawnuwqa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gezflwtbd.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gtzusgsxp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/ghoztmbuh.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/guchndvia.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gfntxwphg.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gdmtffhvn.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gxcmtcmpx.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gpjmchwfw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gefsuilwg.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/grtbxaobf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gvxvxmkxf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gpkdgiplj.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/ghbksiqoq.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gutytrzgg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/glsytefni.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gfxmruphk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/gsxivpotf.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/glkzidbpo.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gtfoujcgo.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gbudbyryx.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gutryrunp.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gtyclqntp.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gvngtcnzh.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gxrsjcwqv.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gfmwpiwob.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gkagyltxn.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/ghhiartta.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/ghxdhnoek.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gijglwmxr.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/geuvuhjpp.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gshqfafua.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gexqgctps.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gjlqjclmj.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gppnyjxgl.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gejawjbuz.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gmcrhsxqh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gzxhpsicg.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gnkhgirkl.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gyklulzem.sHtML


<!-- 参考信息 -->