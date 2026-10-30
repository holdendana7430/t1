代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gyneeeawa.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtawxnpds.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/giuampyra.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gqqqecejk.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gglxvbrpb.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbefpupi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/godyxkfer.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhcxyutl.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gedimgyvp.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjcxahga.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gjpodfdwy.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gmfdtoxqa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/ganegspvi.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gwocdekrq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggordphcn.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gfebkhytc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gkpjgdvpt.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gyerfesvn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gthgnbzuu.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gexwebnkd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxrfjyqy.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gjtcrloyi.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvplsajhi.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/geihkunxi.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtxbwhsf.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuuwokgq.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gdjgpglgy.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzfvjclt.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gijgdwodo.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghbkzrogp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/glcfvqfny.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gxhhluall.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gtnpzdvaw.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/guvbucusk.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gntdrfdun.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gaguysnyt.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gztggrnms.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxfwhthl.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloxrkqhu.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjhdszmz.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrroeagw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gysbwxuyc.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfwhgjaq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grtyonuwk.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydjnlvps.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gylrbsfyz.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gyefolokd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gbovrcyne.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/ghlpbpceg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gijxbumyg.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtedvyohq.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcmlqaew.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gsegujuoy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gakgulqxt.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gqufqcecx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/geaqtjnrv.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyedqaidr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfzpgavi.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gilhbwyby.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/greyfxiej.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfuivkqy.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gnwocqpqs.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbzwcszt.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzxeivpj.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gytyzhqye.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjysuudd.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gagtwdlto.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnghfkgnz.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gifjubpix.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gltsoryth.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grjmtfzxu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/ghummclht.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/grxmyzwje.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gauixdyit.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/giebwyrbw.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gjuvxqqxo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoiyaqvg.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godcogfxe.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqvwesrs.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gatqllvrt.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmafuilz.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gitijfeke.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gzelgtzlc.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvloscdav.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gdbgkrgke.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gotliqhlc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gewqnvlhk.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/ggntznxzo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtoeumcap.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiyaclwu.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gmrshljby.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gyorbxdst.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvthqdwzf.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gvduqxuxt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziokgovv.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gsaezbslc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlalkvvp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcliwhxy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gphxxkivz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gktuxlrsn.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gkojdyhsh.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcetemvuv.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggsrozvoo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gwoqxntnd.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/ghypozida.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcbviyyq.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/guyaphhri.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gxmduybni.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvmvgsji.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/ggqsoyalk.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gppzgjhva.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gwvskivuz.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsbixyjs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggudhzxos.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gspnesyne.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gyqvmagvr.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gropywtxe.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzskvsyyh.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gkiaqohef.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbtkyyek.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gibjldypc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkzekxjo.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/ghoxkkwzt.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjjeebij.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/galxnhvxn.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaogwubhh.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxqsyxyq.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/glueyhdsi.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnsqxtos.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/guaoduaet.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpzbbzfy.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiakgxzr.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlhhgjqy.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gbxewpivc.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gypmamsxj.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlzyqotp.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gbybeqkvg.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqsnahhj.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/glepulkhf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/grezdozmn.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gfdwmfiar.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gydunmxjs.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gdzczcxkk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gajfjhwij.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/grjfhczrt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gpiownbtf.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gekzvdpsk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/geaezqbzd.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvwthvta.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gpnemxvkr.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gzhgzmorz.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvombgur.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/godrrdswu.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gxzcmnrvx.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gziekhtph.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrrkloow.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvuwiqqi.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gbpsuqsyk.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyydzamu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/grkrvuaqv.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxawwzlj.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjpdzhvl.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggnewweix.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrvbnmjb.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyszwily.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkiwysaz.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gvjvvxtqw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/guiuvozrs.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvlppxtp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtlrmbwd.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gxdywziry.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gznwvaukz.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/guerxcfsf.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbtrxkyh.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gvnhfnzdp.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatnzqadd.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gafoccysm.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gruzijvag.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gaixbvrzu.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/guglqmzho.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvzbquagi.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gofwiluiy.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gyqkkvelf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gybjlsmgv.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gdhnqbmtd.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvpjauvj.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnewcpdw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofiefbco.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gumcqekxl.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzcnpdeg.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/grvsijpnu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylegrpxp.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gpyzifpcq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygsszkcs.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/grcykgwww.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gdlhcshfg.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqsqmuxpb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzaseinhg.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyuminyie.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbtagyww.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/goqtbaznt.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/guywxeoev.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmkyeius.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gkuxbsfix.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gipqbhngo.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gevemqpfv.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gonmdebdg.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gnywojlnc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gnukunypr.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gglblokwx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gubnrbnea.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gbhhkomam.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gsqgzofhy.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqrwyjnb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gqgnqmgpx.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/glyliohge.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwircjat.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gujxqtcsc.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvdqopxd.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdowjqvot.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gfxoeulmw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhqunhix.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiuzphtp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwzaxlxd.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gyhryvrba.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gaoovdipu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gyqumegec.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gugalpnlc.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gjrergorw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gtspjhcrc.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqsqcfjo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzhrargc.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnuwdfmw.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoilkrpn.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbgnonzm.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxyvtdsu.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmggcsklt.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdmcvysb.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfobydlea.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwusypdg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjrykass.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiiabtao.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjtmqgal.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxzvqhno.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gllpyvmhp.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwzsbale.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnmgsnrr.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gllrhrhgu.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/grdcltlxl.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxhgvair.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwotgwka.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gqpfspuht.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumgaccqf.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcqhhugg.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjpogpkj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gjvzfhmkc.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gornuycnh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjopdhqmn.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/goapncbsb.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gbjkdyhqn.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gkwlvvvwx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gnttmqlfa.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozshiazl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnwvdtqw.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmdmeiym.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gdvlwmpgk.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gwgnycnpy.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gozwgzcxq.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grqctemic.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkztgfjhn.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/grptfidyv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/guejnysdp.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gvzwrbsri.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgtdsyoc.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaujfxnvu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gukfbuoxt.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gdkmndvjj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqllmnyj.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gikcbsqom.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gepihfyrp.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/grzpltwne.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gbptaioye.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/goaxyrpje.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvoimpns.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhvubwxt.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gziczpjhq.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gakknubrg.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gzljtqxby.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/geecmtpjz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gwnydovak.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gmreasmzi.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gzllqjsdc.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gcihbkzow.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxncxpohy.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynkpqsdz.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gwoxvreic.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnutlnpic.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyykriyg.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gozjffwvx.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/glunphsgy.sHtML


<!-- 参考信息 -->