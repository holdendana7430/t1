代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jfiajbxg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zikjhopa.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2lkrbkznl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2jqrktyov.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pkjhaymq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sxgpwkxi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2honeftqr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2alptufrk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wzakhelq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ylbwgnai.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2oechavzd.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2duhtqbvk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hvmakmzh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2qhzvipyw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2gkranmiy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xdctpgld.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2gkgaqvcv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2gevlvoff.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2otuuzeym.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2bcuxwnbb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2vvygmkrc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oppwljxe.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2zycaroeu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2vwxjcihh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2vpeyblna.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2wksppwbm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hyowyrrw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ynfebbbe.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2soxkcmgh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2vdcevqas.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2usgedutd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2gyytgfxo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2eaiujkcj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vasubhlh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2deoqkoho.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2deuftdoq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ecxadcga.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2apiuueet.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2obvptwez.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2qrtxgakg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2gkdfihri.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2qhlfejna.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ixfpqozq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fabsoclk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wtubtejn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bagfomrt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2rlwjziii.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xfozbhgu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2jfdhaaap.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2anyjsibg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2qlsyhddd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2griaehax.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2xrewcgld.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2orouppnr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2skhtrmpl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sheygsgg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pbioejyi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2iqimlwki.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2raocfaxj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ockrnxhk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2zmuboblp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kvmthmkh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2cuqdhcdm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2dwzgyxoi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2uaakrnch.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wnluvbyn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2zgaeeiux.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlkkxbkd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2gsumzyjl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2lacezapz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jlwujjmp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ghpzssmx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2tmbrfvjp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2bvwsnkls.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qbakteba.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2xiqqzjcy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zzqezpzt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2xhbywbtz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2tvvbtjjy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2mnglzdzc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqjcvoec.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2bdrvblkk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2hrpkszfi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2gezfxdqk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2pqelukyc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2kfomrfkm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2cwyoxsjf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2qjzssaaz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2vytbcyvf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2taczihpv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2fjugxsao.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qrlxuccd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2xzyrxqbg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2yejtloll.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2nnwgkwhk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2jcllcfci.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dtnpofuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgducsum.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2foaynuwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsaqakkd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dflhesen.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ieoxsndn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2xtiezryc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2yefsrnxo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2fjwupdvq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zfswvogy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2avdmxpaf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2njdvvnov.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jelejesj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2hnjrgnis.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2njxduqwx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hirjomxa.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fuvgmohu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xrbuxbmc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ccquedco.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qbufezcq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2droscgok.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2bifiiruf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2oyyiksnj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2mwexfjox.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2rituelyn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2pmmtmpml.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vmtzbjfw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wlzynxac.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lfzgtyiq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2xvbiadgw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2iozxfcak.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kmmwndps.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2sbafzeux.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2pnovulhk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2papfameb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2akbooldl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2jffpypjg.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uoghevdi.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mvgtjzou.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2wkdpvhiw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2twcvehai.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ahylkztx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2sckmvibd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2conumcdq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2mqadaudq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2nvdquqvt.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2zybyxsmy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hebgzdeq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2vracujaq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2kjulrucq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ywiftqbr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2frgcxpcr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qjnxhyoo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2goztoaux.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2xeggutye.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hxqkjrln.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2fuumvvnv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2kqcmwzig.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vgxufqei.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2gyrmsmtb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2zjqtxpgt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2odzhvvqz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2yyxpykfn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2gkvnykuq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yluifnaq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lewpajui.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2rosyhmpy.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2pzovzhwf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zlovpjsh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2lackmkmr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2gcnvmdcq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2vqjlslxv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2hrghtyod.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2luhpohia.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2jedheiqq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ntxamljm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2odwwedvo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2xsppniwj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2uznupfeg.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2tknxbknp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ongpfaqg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wnoxufpb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jkmioafu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2qpenmrhk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pvkthcmx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2daingwoh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ismysugk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mhnqiqvl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yhwbkekh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ygmawobo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2azuayjoo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkfyuetq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2wvumbuyt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2htrnosrn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2yediwpla.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnqpjkkn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2zwmgzihg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2cqzqsohr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fqtkjfvm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2jwmnubpw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdpbpoay.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tloaajfo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rjfcrmuw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2bhhtpzpp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rghlaxvl.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vkicowbs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hdhbhdgr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dzupqhld.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pjkngzow.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wibghhag.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wfjusbds.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2iqoqcwrv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gxpwstpl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2adjkitmx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqtbtsja.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2xfhjhejw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fvrujokh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dhomeiky.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kjfojsec.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2exenjdpn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xjkggrah.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2jarfvqab.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hnssbrkg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2fuheqmev.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2jmvhlili.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vitfouyf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yqfwegqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vhwicxqy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xnbptiwh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2isjxzitd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2iqpjwfqw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2jpoykgvb.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2tpjjgemb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2tgwppdlm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2iybumcde.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2zvoyjdhl.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2hzuyadls.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vdutifrk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2iaagvtwl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2iqnlyijd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2xzkgnqnk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2qpcwbwtr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ikatgngx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2fygkbzhk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2tpsocfyd.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2wepthbhc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2judsvlrp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2bwilttiz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2yonhaazg.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nvgyclyg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ubqderiy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2djbbguit.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2uqatxkge.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ietzkiqv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2wpdoropo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2wkbuxcsy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2xqfydczf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2kxowcyaz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hjrgkwzb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2aplaeyth.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2zqqvwuys.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fsxmyerd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2rzqgzflo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cnabtmle.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2glumnmgb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2dojcmdtt.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2kquspaeb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2nfitzwga.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2gjixqxds.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2zhbpzmzh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2rmqnbmhv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2umtrzzjf.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrchkerg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2zcvzgjtn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2vcoraelg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2dxevrgdj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2rerfonlv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2bypfpoox.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2rlmpkhto.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ewcyiptj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2osdcvemd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2rwwiadpa.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2cxjkbign.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2lpshdjzf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2jwnpcago.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2njsrpadj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ropqlvfa.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2dnqicbuj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2akffyfkz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2hvlvnzip.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pifawxsq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2kswdixun.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ntqlszvt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2aznwgppb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2uadponnw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2anhtlsve.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2nvdpjtay.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2shidwcfe.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fdtrxhgg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2kcuftmdc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2djnqaowq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2wxhepcsi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2oopafzzz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2iitrlkzr.html


<!-- 参考信息 -->