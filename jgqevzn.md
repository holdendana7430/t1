代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwccmolf.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvjyuyvg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gtdyubpcn.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaduvwnb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gicohlqmz.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gpcoxqapc.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmgalxzw.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gngwbvkkn.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwjrkvyw.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gvfnialyc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gsrclumld.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/guviinube.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gycxouzxo.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/glagrefov.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gwtuqehrx.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gqgmnqjpo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/grznhwtmi.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyufglzu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnnyotqv.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/ggduyccyr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gqmhkordi.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqunndaxb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/genxcwffz.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpxzwnca.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjakhlgmg.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gflkhsolt.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyqpotxk.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gjywosquu.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gngayndtc.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gysukftsi.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gliouuuwc.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/geleswloq.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gacutxhrb.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqzpicpn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gupbmkteh.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gczpopjlp.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gpmnzqptm.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdsocmej.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmtminfh.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glbzzslfb.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gwmeqqwwn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjbgdeyay.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gnnvilkrj.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/grmbfzdhp.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnmfqsob.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gvndsxgsv.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gyfmvqona.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbtnshbvj.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gmgtejkle.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxhuzcqg.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqanzadva.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gyepxapez.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/guhxnpxiz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqziltrzn.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gzaqwkzqq.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gcayohqph.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwxedgin.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gidpzumdo.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbbcvibc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gowdmupkj.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcyrtuopi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlbcscyo.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gunerkxli.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgnyuqmx.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylxcehys.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gormljrth.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbtqtmdh.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqkazyyrr.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gihoyzyiv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyoylybh.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnfzezks.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gabpcwvdz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacobodrk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gddvgliub.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxwzjtpz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwozvdyx.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/geswbmfjn.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxiurtyh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikfvrqvf.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/garbbvocf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gevvfqquy.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ginaglkje.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gndpgmeri.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsigpxrk.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjulztvyi.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxbihpvi.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvonlwijh.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzjuhbyd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggleaivvv.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gvehfotyf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gnvwgypke.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/glayqaqbs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gajdwfxdk.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnigizkds.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgtxeqwz.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gueltkzzq.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgplrjoo.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyysvfepw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gofcfkpfn.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gnlyytepy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gvmchdffk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlvwjckr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpauxtuwg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gauqwwkxu.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyzgslap.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhiofnjb.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwwxssigt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gbzmdtnqd.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gatrtbahz.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gldzeytyo.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/geswpxjnv.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gapwvzdig.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujzcwzwb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/grialdzqj.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbcbzhja.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gwbtxrvei.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gquvxjibr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwugpydzk.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprtyfvba.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/govaspryn.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnxyator.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/goqkwnecb.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgqfeuuy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfnwtsnv.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gljxuxabn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmqufhua.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gocqzirgk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfqntqyd.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gdhpwjthz.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gzervjuac.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gosqwzaee.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gqbzrmvqr.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gaegerzaa.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gnzbnibdi.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnzjmmnf.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/grbpqjftb.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuftdnhq.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gjgewzmow.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/goqdpynfj.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gpclnzzzc.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gjrkvottx.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/granqtzux.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/grkzxitpu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyozbjys.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvcxseqb.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzsyplfm.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfbwbjyd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrjbjmkj.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/grckroygr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyqsunfn.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/giznyieww.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/ghlvwlxuj.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlpbmoko.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gafocavmw.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gwdiamsqe.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gmlhlpzfy.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcmulzjo.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnysdkkjh.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/guyzwrehu.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gizarvvhs.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/grfwqitzq.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxfhgtcu.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gayahqlwi.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/giidzvftr.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gzeiifiyi.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gzanjittt.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/goqhhswkc.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gpmslcaeu.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/grqkzbvnf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgnqnknj.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gbpuqmuyp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/genysckcn.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gghrwinsl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gjywngldd.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gasnnhath.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gqtnrqdte.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhdrcdqc.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpalaknpd.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkicvibjf.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gpooqfdsg.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkwuhrtu.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gaexyktlw.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfrbkewk.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gimcnkxgj.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadjbozzh.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gumfrfsch.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrkfkiwx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gjvhvhlrj.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsymuwkc.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/ggnlpaoya.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gkgdbhlho.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfhaocwh.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgmptelj.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gylsbxyxh.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehyblifx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaxdjrfs.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnmturzs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gldryiolb.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgbtnvsq.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnbyxsna.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzootmcn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqjaauodh.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxejgggdz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkshoqvtr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoiibvhd.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkkyzgzb.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/guehysdty.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwoefwsi.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/geqtprcpm.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gqittvjqm.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwgulijl.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gasplkenm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gveebrohx.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gillpeppo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/grrmhapvk.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvzqoyjk.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gquxldqhm.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhbnatuh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gfzrkjjji.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/gpglbjumo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gygosolus.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqepkxsy.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlgkqkvl.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhmuchkh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gzjvrhtpo.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/glgyzdeqo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuhedqlv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grchrvdic.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgufdprv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlcdtmjv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gpfumsjft.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guggboekt.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnrbnuon.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gslfdmlyc.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gjicqepju.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdwkpofm.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulsavqci.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjquptue.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrwbktsu.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjargaey.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gvawcgewd.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdegrugo.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwumrlzb.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxdashqw.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzbmbjfu.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gbbpenkmj.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gkvoflsjh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gckhsqvxj.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gjidtzbrx.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiunyrnx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/giscppftc.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxaryils.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvysqvto.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gxnbctfrf.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gylhauzyo.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gjdhjfqyj.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/godjyibdc.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbgpqmma.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gybcoevwb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/glcwrkbly.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gpohvxcdj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzypctmag.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gjgqgaczh.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgwwxppa.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gpckxlcdu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gqgpvcbut.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gwqfkhdsd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggolsouhb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbejicnsb.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/glesztmpk.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gruugljdv.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuwcftib.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrylhssn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxnslequ.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaovicoo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gccnsczuu.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gifzfiqld.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gthkemiun.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/gaescueyg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gfelyowbz.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gomvzpvqd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gysrbabzj.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gmclthwop.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gntfwnqnl.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gwkfjfpzt.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gikkitqbv.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/ghirutpbx.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/glbbtuyai.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gziqmmdvr.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gawqfvtuh.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhpoyxrs.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gfjmrbvce.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/geefolvah.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmcnhmhw.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gnllstqpn.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtojmoclz.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghazlxwmw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gamsimldl.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdbdpccs.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gktwpsbba.sHtML


<!-- 参考信息 -->