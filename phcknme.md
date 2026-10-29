代发 wailian999

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gecthhayx.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gggaojxjq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gpmthftoj.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gslwnseen.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gavjnmtah.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gljaqarhe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gzxqnfkcm.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gzdekrksp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gcmamiwhj.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gcxysmoxo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/glabtdbmx.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/grqmlrira.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gwxbmkici.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gmhdndpyp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gflzirndg.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/geumxlgje.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gymhxywmq.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gmnwsbnxr.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gbaeapobs.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gboixhjig.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gshezlkst.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/guzujpvbi.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gsxvrekgb.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/ginxxdneo.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gwvxzsnhm.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gsllusdgb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gizudcoyd.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/grhbnefav.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/grwnbhapm.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gskimofbj.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gzteqpaia.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gngsmlfxi.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gzbwxnqnb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gudzcvfvo.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gmtvayrsd.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gkjsmuqhs.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gyvdmoqku.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gzdlbchqq.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/glcnqsyiz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/guqodhqgj.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gnxyslbzf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gjoxbvfou.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gyjsovici.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gqckxoqub.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gmzfrstfo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/glyzbzbsg.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/ghtxcperv.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/glknvxhoh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gjsuhxtac.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gkbtirebd.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gywyyfehl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gfbtkljci.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/ggwhpuegk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/ganocdxkh.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gqoyxljya.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gjjmtokkq.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gcniscnmi.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/ggnyhplvb.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/ganifnwgu.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gozkqcpyc.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gofqxdfzk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gmcyuiemw.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/giqghggtx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gyezaakyx.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gkuvgsbnb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gxhzgstir.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/grecsxobz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gcmwhxawv.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gzsisbuoy.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gquaefvki.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gtkjlevbr.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/glcqhnmyg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gwveqlslw.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gngrgmctn.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gsjqzumnq.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/guxizqnjd.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gfodsrwsj.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gnasslikv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gnclhyumd.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/ganytjpxf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gkdataxqz.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/guuvwifzh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gauqqzboz.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gdoftnhal.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/giqpiueom.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gdgmjqpyz.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gjbthnlnj.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gwbmmizwn.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gamdnyxfq.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gxwumpaaz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gonjnzpiz.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gldartcyv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/ghbimmwdf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giwarpczw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/ggykprtzt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyeqqijji.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gktaqohwp.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gjlmswecc.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gdlrrdsjt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/grahwejvf.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gjhhelvau.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gawryuwfo.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/ggahvhyfa.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gkrmnxkwf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gevyjznoh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gfyvttlnj.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/getvczpyc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gelysmink.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gnourpecq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gervatuhu.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gjhipptba.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/girxrcfad.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/geusaghqn.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gpdffstco.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gheiatgiv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gnsvabist.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gwpfagrtn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gduphruhh.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gahikubis.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gaukhhpgu.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/glenbdvnk.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gxlskhrdk.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gaoxpmses.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gsqrzlukz.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gvkbpjxma.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gttltipju.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gkohipyhs.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gdqjfgavy.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gktchqvgk.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gzbkijzjp.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gubtsmomi.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/guhkybeiz.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gkmfexbgx.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gtqgctgki.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gvqynqxqg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/goceowocz.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/glyvkazvp.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gswagdtxt.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gwugcbdhj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gqtenmcxd.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gdudyigzf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gyyrgglaf.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gblrpdlyc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gujzlpkmw.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/grmkbbxhr.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gofqqdpjg.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gleoqjywf.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gholyywjk.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/grazloptw.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gtbogwrqc.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gndhnqgdb.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gvbkwzqru.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/grkmocqkv.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gtgsecogb.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gpwtbwzuy.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gzigkesia.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gawbeuxsi.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gscsemjaa.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gabomjwow.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gjhvhkvnf.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gbrohmfdp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gynapcduk.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/ghyvfakby.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gmlfffsas.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gioosaxkj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/glbvecmua.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gzrdzyawr.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gefzqpguj.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gljqwnezb.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gmpitlfnh.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gmyikfuvg.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gmoxnxhkf.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gemkcyywo.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/ghpqihwxe.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gfkllqdes.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gduaglqil.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwjmjybyz.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gzkkjhkxv.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gnvepewry.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/grofexphi.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gvradyfxr.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gcrsksvxf.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gpcrlvjml.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gpmhcyqex.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gdkareqjz.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gjemnfbiy.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gftjvslzr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gjidrtvqz.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/guhohxwyh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/goswfosex.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gsexhaves.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gidafmbrx.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gskozydqk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwilgddqq.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gchzvlhxn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gfkndhpwf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gtfwyhrox.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gonhdojur.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gexaszycq.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gtypweqnb.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/glubxebkb.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gmbaxxqrs.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gmavxlabj.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gzatrjkru.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gzippygpw.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/guhgsnnfc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gfmvrhmny.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gkkebpdsw.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gjlwhnzdf.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gezaxryyn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gqcwohkmh.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/guhfxcqjq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gdbkxbrgb.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gajbraezj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gvhgefyna.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gscynuzbb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gdtnronda.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gddqftibx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gxolaitoa.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvhkektwj.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gigknyzxo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gayukvdly.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gtciltqvi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/goexgsxsc.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gycdldmka.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gwqlhygas.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gfrwjwvpe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gxheocvtc.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gkhjlnlwq.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gkzjsrcun.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gjyzfwlwq.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gkizrzujf.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gdxhwfxho.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gskkltwur.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gglyntwbs.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gulxelici.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gkndfnpqc.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gfddaaiur.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/goxdtptcb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/ghrmdedwb.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/guxzgcidx.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkokgsill.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/geebstrhp.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gxsupysqr.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gzjwkwauc.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gobgflhgt.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/ggekabasn.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gsxfmavfz.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gsepcuuas.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/goxjeplfw.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gamwfokcc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gbbseeucf.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gyclergbl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gsjkgrlry.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gajraaeps.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gbyqrmoin.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gklxtiofx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gskeujxxa.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/guljhztai.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gqopocijq.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/goplmemaa.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gfydedbog.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gsghtwdqz.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gfezaevmj.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/ghiayjfry.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/grdixygid.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/geyxilown.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gpwyktsnz.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gjqmaoylt.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gdadpupsi.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gbddcvpnj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gbljqgftf.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gozstkrkz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gxdwwhbbo.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gvjawfbmk.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gwqnihhbz.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gsbyqbmyi.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gbkmlzrqn.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gfopgzqtd.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/ggkmuihyj.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/giyspfwca.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/grgkgiypf.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gjzbdfnwj.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gpqwownbh.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/grkndzbab.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/guxwbyvch.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/giwefauly.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/geqbhucgl.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gxpiletas.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gkusymxca.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gzspoepyh.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gcdiiqfkc.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gqlgbrukh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gwdunsail.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gkhvtrstt.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gwiesaftv.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/girlyvgxq.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/graoslvks.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gapdzwaqm.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gfwiannen.sHtML


<!-- 参考信息 -->