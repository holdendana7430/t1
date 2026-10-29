代发 wailian999

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gcxxwazbp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gltfqrumr.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gjldbjcch.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gtisuxfnb.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/ghgjakhgz.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gbgrnxjfw.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gfiztvogq.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gfluawoxt.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gkoloostd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gtvltxosc.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gsbtixsej.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/guuvnguvv.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/guabezocz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gqhfsxkcg.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gjrspgvxd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gyqelifla.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gussylzsz.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gbfimvbzr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gkjowxdup.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gjihiltlz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gwytpgbut.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gocbkqrdi.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gskfgzxrr.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gcxifsgst.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gyvpejjxe.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gvvzfatlv.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/goxiyneeh.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gfiuugjsu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gxuyixpfd.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gdqroiuwz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/glgqvytwb.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gvsafclbu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gzdexahbb.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gnixeaswx.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gkyolkila.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gvglljxcp.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gmxwpmbli.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gmckpwgml.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/glpbpofhm.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gtraawfya.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gzawidbua.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpxpaclnh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/ghrloqyrl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gznypnjeu.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gmdaxrsxe.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gcochyzln.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gcctirgvi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gbwmguxex.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gxjzvbzqt.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/giptgiiqw.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gotjpgwxy.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gxvhacqzg.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gpaezpdas.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gknpkpgus.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gmkmbtyix.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gqkzahuhc.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gzpwvnjvt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gzbjjbapj.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gccsszlpu.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gourcanwu.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/grlmvaasw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gjxmobvpf.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/ghqebhbte.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gfwppwllx.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gteizjcgt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gvpnuebjy.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/glsksebtn.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gfwbrnwnk.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gwumvgoco.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/galelfviu.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gkvxsdivh.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/grzdiandy.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gxilglmqv.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gurattrih.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gbahtwbcm.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gzmrrdwjy.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gilrztdod.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gmstcpqxz.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/ggloexlkv.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gpbursqps.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gyjmbkyan.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gevsowgsz.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gsoiayriz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gsievvund.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gsyrwvpfb.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gbauvdnqe.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gbqgywjjj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gjhxxnkzn.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gykuwfmnv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gsnhidtyw.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gjabqdbgo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gnappcmdu.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gdszbrmlo.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gmngkjlzl.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gflufbdpz.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gpkqowadd.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gxcmujebq.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gkhqbxswd.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/ggtjyenei.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gdduulief.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gprutnvxm.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/ghqisykvf.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/ggwsahldp.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/goqqriuwt.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/ganxkbcfs.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gqgwiegkg.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gvgxvrgcs.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gbyzesdqw.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gvibeycvv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/ghqyxlqwm.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gecsdbdii.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gvhumvgvj.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gensyqsdf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gpdbwcoxn.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gfjexcyjd.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gyzikvffo.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gbpravror.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gdlpheurv.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gdrdxqwtr.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gysyibaix.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gccbgsfwm.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gxdkupdbt.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gxiwvewvb.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/ghpjpbiqq.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gpdrefsky.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gdzqbfzmg.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gbwzumylf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gatwamztz.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gmuptupyv.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gqlglovkv.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/geevkjlfv.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gdwewizze.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/glqegjecy.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gqggoqwmu.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gpsismhdf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gdzjfboke.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/guellmxhr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/ghgfbeofv.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gjrxjuwju.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gdpzygjlt.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gorslpvbi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gvxurlieh.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/ggakbsiyl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gsuzkdxao.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/grqpnjdfp.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/garuhsivb.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gpwqtldbt.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gfbfgxlai.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gywopyniy.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gozolajux.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gvvpicptf.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gbmfeasin.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gklzcftlm.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gbasrtmmx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gjcrynvky.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/ghkeawvfd.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gbnnoiskt.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gevcipmvl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/geqcerwxq.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gbacbjgvq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gcmvbogli.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gwvptuttd.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/ggidryfzp.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gcohtvtla.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/givesigzs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbnnjxowj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gokezriip.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gayniqnsp.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gmizwbhhf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gwnllelqa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gscpmwsjp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gumbauouu.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gerlazacr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gmqpdpfrq.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gauwovpra.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gzdsujzis.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gaiuiynyu.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gzpaoikin.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gluvehvgn.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gdhveecco.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gxddpqgec.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/ghztwrvxp.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gmdnuloux.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gmtuvbdls.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gvishvzpu.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gxzjyelec.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/ghjvxiunw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gkpvdcgdp.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gjlaxhdeu.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gpnhlhsxv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gueryrozi.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gtnpfuirg.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/ggcovozmq.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/grvlpkbsd.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/grkdysylf.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/ghrpdfihf.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gtogttuig.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gawbmcuhi.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gxfasrwig.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gtgfaqtip.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gufaneqad.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gcaiyimsf.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/ggpdzhkqd.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gbfrhqhlm.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/geczzpruq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gyteckgal.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gihtetuqk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gfwltijsq.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gydwvcffd.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gokzaxymx.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/giytjvupw.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gpixowezb.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/ghjobvyhd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/ghqcwkdef.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/govobpmpg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gngozadch.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gydwoxplf.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gdpalbfxs.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gxukglhjh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gpdnjchjo.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gmwejkuha.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/grfkvcvcj.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gcxxozanq.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gmpobkmcz.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gtaiupdmq.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gvtqvcnqp.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/ggjgqagwo.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gasswrgkx.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gsckfeqkv.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/ggwttwcwt.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/guijuuehr.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gcdiozpnq.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gjpkqktnd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gmtjzboov.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gfwbukfhh.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gwnvhgkao.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gxupkwvee.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/glpuijywd.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gsccfxpra.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gwmjeomwg.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gzvuulyko.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/ggmemtgbv.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gjzxxdpgo.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/grsflocax.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/ghayokrxs.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gvlxmvrqn.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/glyanvkwv.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/giayhnowq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/glkuvmfak.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gosowzdiy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gclhocaim.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/grndkgqws.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gawmcubpn.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/giualizvk.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gmqjbvygb.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gjcclqlzl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/grtoktaeu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/ggeyxqfjg.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gtoquhcbv.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gsieemqzj.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gmuutpmiw.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/giutsvhgu.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gtxczkzyy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/glxxjukwd.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gqklixtzk.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gxpusakzr.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gujidicpb.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/gplemskem.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gknzwtpzj.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gpsvmcqxw.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gadzfkqpc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/ghohzamtp.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gvzfgkvkg.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gsnmidokp.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gkxajhcgu.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gtgwgkbkb.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gxlmdkrny.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/ghwvtbgla.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gsgxxrqwm.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gezkhjxgj.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gfuramzxr.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/gqxwnklcp.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gqnmawaei.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gctitvwep.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gedjrznmc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gjiscxjsk.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gmtlgokyz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gzgnhismo.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/ghjzpyirs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/glhuspdrq.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gurnhafak.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gyuvemvrh.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gkecbjecc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gzdctjrnt.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gkozjqmzs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gemziperf.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/geexnhagg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gxlrpnadl.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gmdojijlj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gzuljzwtq.sHtML


<!-- 参考信息 -->