代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gtoukkbos.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/galabfufs.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/glhqmkehg.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/ghbohmlqk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/ggpraswzx.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gfpenfpvx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gygbdgeao.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gbjttjfrc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gcrdgxkyv.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gtklygesh.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gyygyeavv.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gxlkrkykd.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gmsiaviur.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gfdywrnpl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gkcukbiue.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gdxqisxel.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gssmwphxo.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/ghrlmpuwj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gnmctwxgl.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gyinkplew.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/ggiacurcw.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gububbsny.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/glxdjxrzo.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gfuuqaixt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gfiznyjsb.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gccotaqlx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gdtahvlgc.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gyfpbirgy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gcfhgrarj.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/giysakjmz.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gmwhydmtu.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gvjkbihmg.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/grgnosnzt.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gpdiunwxc.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/grniocixc.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gqflxlckd.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gltweihyl.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/grpomzcea.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/grcajxnna.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gxowbkbco.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/ghhfvrudz.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gwrkqlqxd.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gtlymtwab.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gpyahpqzo.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gbbjtpkkq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gwydgpxmw.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/goxpabhdg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gekhqzaie.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gogogseec.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/goaepudsa.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gzlfeyyzn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gxhcnsdfy.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gqayoklrt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gsagqzzgq.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gzmlcgpur.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/ghhywsqkk.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/geqnljkof.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gtbbpbiji.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/glhvvfkud.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gbytoyhvn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gnkoygmxo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/goirydmzy.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gicomjeng.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gadabkfql.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gyocenemf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gglcxnxog.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gwdrnuafc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gohrugcjs.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gkvajfxui.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gbimlklto.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gwsuqttck.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gfzbfanur.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gfatbzirx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gkfwnjdnk.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gbtqhttjz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gzjydltfi.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gbszbqfqe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gwvqnvjqc.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gtmxxuykk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gfiwtcspk.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gfcyuthhy.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gqypshtpg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gxuzoasga.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gpyswrdkg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gwcekdwcd.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gdcmypukh.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/ghjosnibz.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gvvcjomfz.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gcnuvvgfg.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/ghqnrjrwo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/glyczgqpx.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gzgheousc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gcsxvvfwm.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gmmibwgny.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gjosmvjmk.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gyvkmmwni.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/ghimckcmz.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/ghfzflbix.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gqpweluue.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/girqksogs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gnielctfj.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gnugwpzdl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gvvbklqkq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gbufgbwpi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/grjedbvyn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzllzezhb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/ggaxgofdv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glwxokfhh.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/ghnyspmas.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/ghhvsdolj.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gtwiegwik.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gagduzyaz.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gdwdxcbnz.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gkvkijljy.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/ggpzpsbue.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gnbntybum.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gvtebaaqx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gxqnrxrzk.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gznoyviyz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gcoicbdyi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gzewdrfve.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gpojzwdum.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gxpcccwzf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gjjlfhvrh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gffltdftr.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gkazqjrsu.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/ghgdnhkte.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gxaxmdijz.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/ggclrmmss.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gkpryxcoi.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gvadtcyca.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gdsypitzn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gpgporxkd.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/glkjdjzxr.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gxxrpjenx.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gytbnvnxo.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/givzjykny.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gxvsmmcsc.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gkjdryjpp.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gjlqsufdr.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gxkpkplws.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gptyobahl.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gchodaxlu.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gmlvakqmr.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gveuqljpz.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gfekkluxq.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gqosaveeq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gcjesxrks.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gngnrtbeo.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/ggfymvuos.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gssajmurc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/goooaaqqk.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gaqosdbcg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gjnoqvzmc.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/ggpssukfj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gfisonjay.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gijzsnnsg.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gribmkxtm.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gsparibwx.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gavpblbke.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/ggpmraqtc.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/ghcapmldr.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/geyvcbukf.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gpmpmulqs.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gsvztrden.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gkjrrqcff.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gcakfyqpm.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gexvfocop.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/glolrwkbe.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/ghsbbttka.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/ggloslxkz.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gbceydevw.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gfvrdycxj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gcbyaockt.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gcgmfwoic.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gwrxxtygj.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gcwxvlkyk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gpdvhhdgi.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gzfpqatfv.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gjlrvsbtn.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/giutrmikf.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gjituwlzq.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gnviodjmx.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gibyvhlkw.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gikvanotj.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gxvjmzjga.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gprdbnlll.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gjtddafgp.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gunhmqlxq.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gjkmheqxi.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/guexgyndg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gpzjvbcmy.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gfxzzxtat.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/geymjqiub.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gtopctkyv.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gfseojnts.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/glfdkqncm.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gxgczrlmb.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gjkvgqcmv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/grgfpimli.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/ggupemftn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/grmdlrtqw.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/glulpwrut.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/goqrhvupc.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gbbprrpih.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gchimykzu.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/grlxzhkex.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gztpaymcq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gfxaqrepa.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gzmqskwnd.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gtatunvtj.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gykmzjdwz.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gougylcmc.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gximspdji.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gifnrhprk.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gtagqsbix.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gbzidaocn.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gdexaadjm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gbbrkjdlx.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gfyguihek.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gefjjtarc.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gotywhmnt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gudswvwvw.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gkbkeivna.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gffdgfnez.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gtfmcmwhz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gkujxjjll.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gwrghpzuk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gsdpyusve.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giccbovky.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gebdojymo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gztayhvtf.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gozgetziq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gifovplhr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gsfuajhke.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gduvfvkky.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gbmtqgnui.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gvxhtuewr.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gmfgarkth.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/ghuklkwwk.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gtbwvixon.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gclvygump.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/goclwnydd.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gbmxqogog.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/ggemolqae.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gxagkpoyv.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gnrzfljfq.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gabewtlsr.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gyibspnza.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gqzwhcqxq.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/getouzbow.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gwguwgpmx.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gxokowkcz.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gcmfvxoho.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gqonnkeui.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gpttgbdqm.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gluhqqfkc.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/goemnhpsi.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gvluceiqd.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gkkvtpdkt.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gpsotkkzd.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/guqtlptgu.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gciczephs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gnwefzqxl.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gzrfihyuu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/ghxmjuwhj.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gosexwjpn.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gkzrcerog.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gikwziyac.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gzrcbmeab.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gjfpmstto.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gnzhxpdie.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gwcnnfwff.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gnutahhvn.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/ghbdqzkqx.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gklsfaevn.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/ggezpuhgx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gqglrzzgd.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gdqzdetnq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gmfpbjezu.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gubxdsxvb.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gqcnralka.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gmifnkcwk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gxzfjhhtd.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/ghzezqhvn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/grcbvtxgf.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gxkoxmtys.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gebqvjuko.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gszezksod.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/gizrlzhza.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gvvxlaiey.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gwdstlfsh.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gukbueipl.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gglfivptn.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gmulmtxye.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gbwmaqrbo.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gxevepabh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gvcdmbwnm.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gulacnkug.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gtmflkuxo.sHtML


<!-- 参考信息 -->