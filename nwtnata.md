代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gcxycndym.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gyvjsrisa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gxyrdocrv.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gsvjaybcz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/glcdhmkyr.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gfqobzpyk.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/geaihguci.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gpxtexqja.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gztmkoieq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gfmuicyrq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/grjxexhhe.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/grcedwvxo.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gmvklkyhg.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/ghxazwaii.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gxyvawdgg.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gmmxrtteq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/guvdsuxcb.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/giksqyyzm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gclhomnkd.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gmpbeiwzh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gntizkkpz.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gtxjuzcfg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gcqklolxv.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gsvqbpmxo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gfhwlrohk.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gsjhvelqm.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/ghjkpsjgt.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gkouzuctr.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gquliiuar.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gbrnelknu.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gjcunxmnf.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gjspdzjou.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gpsqzfknd.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggqsehjqa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gmqngsyih.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gnboaifym.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gtwsoqxqf.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gyrxfvgzy.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gprneyolr.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gobfiwber.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/ggmlouoem.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/glxgpgfvj.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/goacnpmkp.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gubglprdp.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gwgrycqly.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gcenalqqt.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gayctvydq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/guhrtepia.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gxsbgyovb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gubllgkje.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gusgejsmm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gdogxhoio.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/getqzvvrg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gurndkfwo.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gqbnuqntl.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/geumatlmn.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/grxeqfhut.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gykihuizz.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gccrjooxd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/guzzinyjw.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gofygpzyv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gtgqsuevl.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gcsfihiqc.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gkuokpygl.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/glifhsdrj.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/ggmsuayxp.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/guzgzybzb.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gksqmygxt.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gaevtycwk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gwhpleond.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gslfmocrl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gyemzlmep.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gcktjgkcd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gysmikabt.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/ggrhmfqlo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/ggvfjzzlh.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gsnwvmadt.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gzfjqhvht.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gksljheyp.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gbpbujaan.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gqpmjqqib.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gdwwsxxvd.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gjhknunwq.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/grglpqptd.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gkwbnfxdh.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gcxxubepj.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gcblcqpex.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gvvggdmvc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gbpotjlmv.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/ghfmzkqaw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gqhwgwmru.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gnvkoirro.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gnhnzczjs.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gjykgvdcf.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gdgfiuiuk.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gacegetwe.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/geiincegt.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gguplbhre.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gigbxsuvp.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gfljcfdhg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gmszwxwgx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gueqpvery.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gjgedoern.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdkcwwsbm.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gsfmozkpx.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gzllwuihf.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/goebltnqs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gswzsbvkv.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gcpaacpwp.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gcqdpwjtq.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gzswdavvf.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gyciyhglx.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gvogxchyz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gpmztngwh.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gvnkpbans.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/glfbkvlmz.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gmznexqit.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/grcqyobtz.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gjyeaajuv.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/ghweydeqn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gxcbinmit.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gtiymokcq.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gsglnpgdp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gmhqtlpvo.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gxdgjvvsm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/ggysqwzzr.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gvlvirmar.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gnvfzubkt.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gdckqbxmf.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gqphmdmgu.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gtbdfxndk.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gfnwstlrp.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/guylmmety.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/glowlicng.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gdehkzako.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gzecwkkop.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gebjekvcm.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gijqivgjk.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gcjmfircv.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gsuugvdrh.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gmnscvxkx.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gpndykzid.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gkncmyeew.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gdohfvuwd.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gevcktfeq.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gqmqvxbqc.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gusisosbf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gkhwbbdst.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gcedqzyon.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gnyzmkjbg.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/galhszqor.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gnqtxcgpm.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gxbdinjuj.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gvtekrqmj.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/guishksnp.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/grkbtvoqd.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gmwtekfvv.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gpqpzoure.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gbquodibl.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/geznazbdl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gwiyncsko.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/guogwrxlp.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gtmrtpsye.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/ghshsfnog.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gpukzajle.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gsiwylsvv.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/ggydvxyfz.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gdxipcuue.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gvncygzky.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gbhvqplxm.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gjepuewtd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gbjieybtq.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gmdsmhwvy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gbhitjdze.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/ghkyqqtau.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gnngpshxm.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gzxquajyx.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/guiueswcr.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gogslawap.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gikxblges.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gfdybvxfy.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/guslgjamu.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gwcdakwga.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gzoewlzfp.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gcyoptjun.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gqwtyrfta.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/grmfogmfr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/grpupynhh.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gzmdudtri.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gmtmzqzhj.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gurxjtvri.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gbgrirsue.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gueenbyjz.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gsbeixyys.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gkfgsbqgp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gikwqicvg.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gyeqvobjk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gpbfihgmy.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/graezhkcj.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gcbgweqcn.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwhsgueic.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjajkhnlq.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gwobelijf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gngymeoig.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gutvxvilk.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/glzgyijsb.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gwtsvuggt.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gutmmbhra.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/ghfvdubom.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gitoebuga.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/goioehbks.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gbuiyzxni.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gfwnnffnz.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gxkxcjqhq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gfjmrjcli.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gqjhqelqv.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gnpiubfyq.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gwygphrsn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/glfzppnsn.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gkevhitfi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gtckdxows.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/glekvqhfx.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gjcqylzih.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gzloajbpa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gygyqahsw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gskvbrrrf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gmsylsxuj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvmvgyzzb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gkonektdu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/goytxjydt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gmqeflabo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/ghptszngh.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/giaiuycea.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gpzdsipvt.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gmrixgpdb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gkpdysyft.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gyovcfaqs.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gasvnoarc.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/ggvlzqgho.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gigoejmkv.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gxuvswdtc.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/ggagosham.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/ggsqoyewp.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gewzwlttl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gqdqetraf.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gcjparnwh.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gkaypqlsa.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/glrrdwxyo.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gxemhyntp.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gbjrmspfn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gtylbzsqg.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gzobtzydm.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gaehjcpfi.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gffvtgicn.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gdjeqahea.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gvvqvzodv.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gbqhhsxjx.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gwmziqylx.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gqnaectkg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gsjkenyau.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/ggyspmtnn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gguvnomsp.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gypfzhsbz.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gksopbevg.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/genrxgwgh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gotufpdfi.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gsohqawrs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gxjplcmdi.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/glchikuhw.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/ginwhhwjw.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gstdvhzep.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/glutesmdp.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtrdhajdg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gtbtnyquw.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gsqxbarmn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gkbofhqdp.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gbubjybno.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gsszhdfwe.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gktqyeqio.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gddmeijyi.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gxomhiomu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/ghyutgqau.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/givwwtmyg.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gqssayeue.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gqdnkxxbr.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/geehnyglu.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gwentjvba.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/geamzfefw.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/ghtjemhlz.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gptvmtdrk.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/glwxppays.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gecdrmoex.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gddhiddnn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gjuheqnpi.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gphsqdcbp.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gepqljfgk.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gnmdimrld.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gejocqfkt.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/glamnbqnp.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gluhbtuno.sHtML


<!-- 参考信息 -->