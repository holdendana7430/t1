代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3bxwznfqg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3mnbxhith.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jhdowyzs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3zfqsqcxr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vmdgknbv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3kdshyrhs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3zoscvapo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ynfrrkea.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3pmfmgqnv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3onjeoxcj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3mamffday.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3rcuxlrmd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rgpybwcd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tsevpldd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jgwpstyu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3uxgdzevv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3yunxowfl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ixoxoibg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zwtkyksx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wwocolba.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ybijjoie.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dqcfvkom.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3tctlqzce.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xylnjflx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3hxlrqzux.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3gggtyyrh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3gnpppgqu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kwxzzrav.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3fcuexkxh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hsolziqe.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3oipzdnvi.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3rviaagif.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3lzyekyun.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3pjrukqar.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ssibmzff.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3lxwcagym.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ophcfsti.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3zccehexr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3mkjussny.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ndnnhhmx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wfnrzqeb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bgnxdqlm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3nvntgtvy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oigshxpt.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ugdwpjkb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3bdrymklr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hjukpicw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3urjwrgtc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3mxtfwuca.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3xtsnommu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3eoudnyow.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hctkkhsz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3oebnahqc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mwcqmafj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3bytmxoku.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ahpunkof.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3tjxuclll.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3zmxvuyvg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fatnlfaj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3julmdbko.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3euafomgy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ynaivuvm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3rreswwdm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ioalctmq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ekuwbmxk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3oqariuwu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3dcfvkqxr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wjifiame.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3vetzelah.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3janzhkvo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3hygghwug.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3myubrceu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dsmfadlb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3crdjjfhn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3kztonmwq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3cunvpuvf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ewnxbhwd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wzxswxhu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3duljpclz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ojoqiduq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3aljawcsu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3soqinznz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3klihzqik.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3xbamsxxf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mbqgchzv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3oplnwkvy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3rwuzxowm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3qzonwbpb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3kivscaqk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3lhvlppai.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wbqziwug.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3tklqlhwx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gmdvcqpg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wkqmhgcn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3nobabgre.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3flfsvxch.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbcisasv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3aqheoqen.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ntdwofuj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bedhwvys.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xlarkrnc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xqrjfasa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ueokjhsi.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3nwgvfqxe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ptrhxkhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ylgawfmh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mjzmljom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbylgmda.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iidvbfww.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qnwnuqla.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rrcmsrsl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3dmkioqcj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3igrnulxk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ivacjgti.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3jlvthscf.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3dmxidniw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3hitwnhjn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3nwjnicrk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qwcunahj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bgchakpu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nlmxthld.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3xoyswkwn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hbmsskvs.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vtkpdxrk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3xeqgdyho.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3wrpiyjhb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fotvgzke.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3cgffeqdz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3snablzpv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3guiktlkf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3fxpzphlj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3prmpfvsu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cyzvdmcc.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ochvyexh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3afiuohal.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3oapkblyo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3gvfeiczl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3tkwgpmhs.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zebjqnvm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pgfgzyrg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3yymtnmaj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mpjbasjp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jaynmiop.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3sntwucuw.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3hciwxkyy.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3avzqszza.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3cywjveqb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3sazhbrpu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3oirbivdf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3exonkuhs.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3yevdfrpl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uolxlyww.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ppewzflm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3wktkxwhz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3yoevlvis.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3eamtkfzz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3hllzvpwn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3odchstpj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3xjmgltfe.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3gcmvhvrx.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3erqyoxub.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3jojlttnz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hbwemhgw.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3zdevvtxr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3nnqvjhot.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3cffewcns.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3lwghoxml.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gwiwlxsd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ovuniaoj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gdxxrbxw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3axehuwje.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3stdwjzqg.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vjfrpwai.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ffmereqs.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zonwlnlb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3pqhphyub.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3kwnzzfhp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3egtsyeav.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kqopcybn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3aprsofpr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hgxqxyoh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3eauxwubx.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bzkxbhgx.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3jvxnzkwp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ygyimuzx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yoplgigw.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3kbvzqioe.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3zgtozmoh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3grgvstgy.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qimmpose.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gadbojzq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cmcyusnc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3iaacgxti.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3hglhjjnm.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3cykyjukq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3yfrzudwz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ppvheqdi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3plazjlnu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3aaugckfn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3aedrtiex.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3gagdkast.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ykxkgoyd.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3kyrggayr.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3qompypua.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3yonvzldl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qyyxsjio.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lbrpdtoz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wdskltbd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3usxjdfrl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zbazkjwh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hvnkuvtv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vyluuobf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qellybcv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wisnmade.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lfcjaqvu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ymmfbckg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3udorffhz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3oszblnrc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhevzcey.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mwmzibrd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xvunpqaj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hdkoevqk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3kcbmvshc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3agttvfeq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3epyiofor.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qvqpinek.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hkpczneu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ypsljbvz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3cunrquue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxtgglhh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zrkjrwhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zuycrgmo.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3jdacvnfa.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3aqcjxsed.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3eyhswsxk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3bvtwgaro.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3krhhspym.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3nfdevslk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3oxbpyapm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3blfeictr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3tfhnfsqx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yxycgidi.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3cgnieglk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3znajaoxg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ypqfaxhl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3kqewhdhx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3kribbaix.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ertlhbhm.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3vzdwqfjm.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tetmagya.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ewsrkqah.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3jikhzgaq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3kckdzszy.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3obdqeukb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3vgeivccc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xfwbolyv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3frtamxjv.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3alvvjwru.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ubwyoyln.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3bootlfvc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ycdnewnz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3mknyinej.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3slvysctn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3oktjoxyy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3iqrjeldn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3qiatosex.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3jpqluzhk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3iczkuvyq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3dtkkaiou.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3pmkkslwz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3kvsrfycm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3pjuyxryi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3lvmaqmhh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ktepwbpb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3povhbdiu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3glpevobs.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3wpveulfv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3hyvxrqug.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3qqnpsobc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ywqaqzfg.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ampdnymk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ficnlaux.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3npvngbah.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3eapocela.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3alhlcyiv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ymnmuzai.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3rfrytxbj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3udztaakj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3hevipcti.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3jvdtxewr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3jrhftjpo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fqcgzeen.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3lrlazxvx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ozzogzrr.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3puoqjcgt.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3wncbwhpz.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3fvmhujqv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3nlhdeaxa.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ahzidoqr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3kyroocdi.html


<!-- 参考信息 -->