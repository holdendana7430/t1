代发 wailian999

x |= (1 << 3);
来源：http://hz.316326.xyz/gtfoonjnut.html

[S17] C：安全拼接字符串
来源：http://hz.chenzaomai.com/gtdxtwilyp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.birdmap.top/gtcqlfjsfx.html

[S18] C：命令行参数
来源：http://hz.smart0.xyz/gthfqohzwc.html

int main(int argc, char **argv)
来源：http://hz.andypj.xyz/gtbgwdxhob.html

[S19] C：快速排序
来源：http://hz.jqgfzy.top/gtijxyxyfi.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ppjwa.cn/gtnuqpimzp.html

[S20] C：二分查找
来源：http://hz.jinghuilouyu.cn/gtzzylywoh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.havefunace.top/gtazbfbpgq.html

[S21] C：字符类别判断
来源：http://hz.ybcxt.top/gtdhovvgbv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nanxuanxn.top/gtrvinddvh.html

[S22] C：字符串转数字
来源：http://hz.zhixingplan.top/gtouoyfxvf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yonumen.top/gtlivmiqxn.html

[S23] C：随机数
来源：http://hz.hysaishi.cn/gtjnnsgavx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jianghu66.top/gtrsklshee.html

[S24] C：获取本地时间
来源：http://hz.zhongyouzk.top/gtwdppljrp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.aibaodan.cn/gtttpgzwxf.html

[S25] C：内存拷贝
来源：http://hz.0kj1m.cn/gtkrjwfjma.html

memcpy(dst, src, n);
来源：http://hz.iojbl.cn/gtmrjrtwth.html

[S26] C：内存清零
来源：http://hz.shanyushiyangtech.top/gterrtftgq.html

memset(a, 0, sizeof a);
来源：http://hz.52xcode.cn/gtmvmkxglm.html

[S27] C：定义常量
来源：http://hz.cdnleiting.top/gtzdrdjxbb.html

const double PI = 3.14159;
来源：http://hz.shuidangran.top/gtjswapugg.html

[S28] C：静态变量
来源：http://hz.cheryme.top/gtdlcyyonj.html

static int counter = 0;
来源：http://hz.bjfxy.top/gtnaqdiaki.html

[S29] C：变参函数
来源：http://hz.dianchejie.cn/gtykuhnntu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hfpthk.cn/gtdkkcadjd.html

[S30] C：头文件保护
来源：http://hz.ehwqpu.com/gtwcuzarhl.html

#ifndef X_H
来源：http://hz.kuanghao11.cn/gtacbhxpjs.html

#define X_H
来源：http://hz.pycfn.com/gtjlrywmuj.html

#endif
来源：http://hz.ybcxt.top/gtipcxxujd.html

[S31] C++：Hello World
来源：http://hz.daxiang520.top/gtrmswfcfs.html

#include <iostream>
来源：http://hz.gzhubu.top/gtgavhcyle.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tian-w.cn/gtmfhfyfre.html

[S32] C++：字符串
来源：http://hz.hammf.cn/gtqubwmcwm.html

std::string s = "hi";  s += "!";
来源：http://hz.zycfv.cn/gtxcwwdgyv.html

[S33] C++：vector 增删
来源：http://hz.xuanzx.com/gtpdrmkerv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sufxvd.cn/gtbablysfw.html

[S34] C++：遍历 vector
来源：http://hz.chenjidiqi.icu/gttzhibsde.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.wangdashe.top/gtadqzlctb.html

[S35] C++：map
来源：http://hz.52xcode.cn/gtmardgoem.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.andypj.xyz/gtkzbnsimi.html

[S36] C++：unordered_map
来源：http://hz.gogol.net.cn/gtmlfkvgcj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhengqikj.top/gttpqaoksp.html

[S37] C++：set
来源：http://hz.ybcxt.top/gtrajozokh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gzhubu.top/gtrmzehwwi.html

[S38] C++：排序
来源：http://hz.andypj.xyz/gtjxrhbpir.html

std::sort(v.begin(), v.end());
来源：http://hz.yangfankeji.com/gtpvbvmeqq.html

[S39] C++：自定义比较器排序
来源：http://hz.guannengcc.top/gttuobubpr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hammf.cn/gtrjnbwwkd.html

[S40] C++：查找元素
来源：http://hz.yongpay.top/gtetvdiktj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.quarkkingdee.top/gtparuipjo.html

[S41] C++：类与构造函数
来源：http://hz.ywan-chungtsiang.top/gtptyguwwr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.guowangkeji.top/gtcdwsnrdv.html

[S42] C++：继承与虚函数
来源：http://hz.jinqigufen.top/gtojtikyws.html

class B : public Base { public: void f() override {} };
来源：http://hz.sxryk.cn/gtcyzgwrro.html

[S43] C++：智能指针
来源：http://hz.zhengqikj.top/gttplqypfq.html

auto p = std::make_unique<int>(5);
来源：http://hz.xingfuxueyuan.xyz/gtfkkbkwrp.html

[S44] C++：引用传参
来源：http://hz.gotoacloud.top/gtcclvijss.html

void inc(int &x) { ++x; }
来源：http://hz.ybcxt.top/gtboehyxjh.html

[S45] C++：lambda
来源：http://hz.shanyushiyangkeji.top/gthfhawkqe.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shuidangran.top/gtccklgsmf.html

[S46] C++：函数模板
来源：http://hz.aibaodan.cn/gttidhsocw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.redwolf501.top/gtznjjgbbn.html

[S47] C++：结构化绑定遍历
来源：http://hz.cashguo.top/gthhxwrqyn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhongyouzk.top/gtrsdesczr.html

[S48] C++：逐行读文件
来源：http://hz.yueranfly.top/gtgmrdwqav.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.feifeiyinyue.top/gtfqxaaizx.html

while (std::getline(in, line)) { }
来源：http://hz.xziqi.cn/gtmlvicqhn.html

[S49] C++：写文件
来源：http://hz.sweek.top/gtqxaofcar.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhongyouzk.top/gtueejwrtf.html

[S50] C++：格式化数字
来源：http://hz.jyoumei.cn/gtrkmqwfmb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenlongwang.top/gtxmmalcij.html

[S51] C++：显式类型转换
来源：http://hz.chenjidiqi.icu/gtcvlfbifc.html

static_cast<double>(a) / b
来源：http://hz.sxryk.cn/gthufbsmhu.html

[S52] C++：const 与 noexcept
来源：http://hz.meibo888.top/gtstfnhexp.html

int size() const noexcept { return n_; }
来源：http://hz.fengsongda.top/gtmzllrflx.html

[S53] C++：移动语义
来源：http://hz.xuanzx.com/gteoqsulbg.html

std::vector<int> w = std::move(v);
来源：http://hz.zdqjudy.top/gtexnswdep.html

[S54] C++：异常处理
来源：http://hz.cheryme.top/gtaehkfrbd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.pycfn.com/gtivtqntdq.html

[S55] C++：结构化绑定
来源：http://hz.zdqjudy.top/gtuexgajxj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yonumen.top/gtyshwojpb.html

[S56] C++：optional
来源：http://hz.bjfxy.top/gtvyoxmaqo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.wangdashe.top/gtewrlcwtj.html

[S57] C++：编译期常量
来源：http://hz.ywan-chungtsiang.top/gtyqlyxqci.html

constexpr int N = 10;
来源：http://hz.gaohongyu789.top/gtlsfsvipj.html

[S58] C++：命名空间
来源：http://hz.zhixingplan.top/gtsvutzzwj.html

namespace ns { int f() { return 1; } }
来源：http://hz.cqqwz.cn/gtqxtbjaim.html

[S59] C++：静态断言
来源：http://hz.xylfe.cn/gtbzwhmbtf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.bjfxy.top/gtwmnyleyj.html

[S60] C++：遍历并删除元素
来源：http://hz.jianghu66.top/gtjellduzn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ydzc1.top/gtenisymfd.html

================================================================================
来源：http://hz.nanxuanxn.top/gtancdehyj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pycfn.com/gtylynieve.html

================================================================================
来源：http://hz.tanke756.top/gtykmakkui.html

[T01] Kotlin：Hello World
来源：http://hz.sufxvd.cn/gthziqzcgy.html

println("Hello")
来源：http://hz.xziqi.cn/gttvkxzhtd.html

[T02] Kotlin：变量
来源：http://hz.hysaishi.cn/gtftwhsfpr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yueranfly.top/gtsuiuyhnt.html

[T03] Kotlin：字符串模板
来源：http://hz.ybcxt.top/gtabzzlqcd.html

"值: $b"
来源：http://hz.yvedp.cn/gtxlznjgnh.html

[T04] Kotlin：空安全
来源：http://hz.yanxiufei.cn/gtjepkmbzj.html

val n: String? = null;  n?.length
来源：http://hz.ydzc1.top/gtjlxdiedq.html

[T05] Kotlin：when 表达式
来源：http://hz.0kj1m.cn/gtvijjklvc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jqgufenzy.top/gtqbzpgokq.html

[T06] Kotlin：集合映射
来源：http://hz.shuidangran.top/gtfstvojnq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.redwolf501.top/gtybpdkjkf.html

[T07] Kotlin：集合过滤
来源：http://hz.sysykeji.top/gtcegxtqpp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jqgfzy.top/gtosvflgtg.html

[T08] Kotlin：数据类
来源：http://hz.yj20258888.top/gtvlfrjxoq.html

data class User(val name: String, val age: Int)
来源：http://hz.yangfankeji.com/gtrqqeglhy.html

[T09] Kotlin：扩展函数
来源：http://hz.zhongyouzk.top/gtbehuxhsj.html

fun String.exclaim() = this + "!"
来源：http://hz.havefunace.top/gtwxzqvjvp.html

[T10] Kotlin：默认参数
来源：http://hz.hysaishi.cn/gtmdqpkxok.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shanyushiyangtech.top/gtyndeobxj.html

[T11] Kotlin：协程
来源：http://hz.zhixingplan.top/gtnftosjpt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shanyushiyangtech.top/gtmqjdcikx.html

[T12] Kotlin：解构声明
来源：http://hz.xziqi.cn/gtvwsyzqve.html

val (a, b) = Pair(1, 2)
来源：http://hz.ehwqpu.com/gtfesqtfnx.html

[T13] Kotlin：只读 Map
来源：http://hz.zhixingplan.top/gtgronpjfh.html

val m = mapOf("a" to 1)
来源：http://hz.gogol.net.cn/gtghhmwgin.html

[T14] Kotlin：循环
来源：http://hz.cucudq.cn/gtkbrpjobd.html

for (i in 1..10) println(i)
来源：http://hz.pycfn.com/gtkirbxsvv.html

[T15] Kotlin：接口
来源：http://hz.xingfuxueyuan.xyz/gtrypuuihv.html

interface Shape { fun area(): Double }
来源：http://hz.ehwqpu.com/gtnmdsjevd.html

[T16] Swift：Hello World
来源：http://hz.iojbl.cn/gtlrgiojsu.html

print("Hello")
来源：http://hz.cucudq.cn/gtprixoscp.html

[T17] Swift：变量与常量
来源：http://hz.xinyue.icu/gtlduxyfqw.html

var a = 1;  let b = 2
来源：http://hz.pycfn.com/gthldirvst.html

[T18] Swift：字符串插值
来源：http://hz.nanxinkj.top/gtordlbxsx.html

"值: \(b)"
来源：http://hz.chenzaomai.com/gtsrmbziqs.html

[T19] Swift：可选绑定
来源：http://hz.c1oappe.top/gtkizvdatu.html

if let n = opt { print(n) }
来源：http://hz.sweek.top/gttgrzaeon.html

[T20] Swift：数组操作
来源：http://hz.tian-w.cn/gtvvrcjmrx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hywenlv.cn/gtfvapksgx.html

[T21] Swift：遍历
来源：http://hz.jqgfzy.top/gtucpmophg.html

for x in a { print(x) }
来源：http://hz.smart0.xyz/gtqnpgxopo.html

[T22] Swift：字典
来源：http://hz.cucudq.cn/gtpphegcoj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ybcxt.top/gtcrveijth.html

[T23] Swift：函数
来源：http://hz.nanxinkj.top/gtwptvlpmp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.gaohongyu789.top/gtjmismieg.html

[T24] Swift：闭包
来源：http://hz.0kj1m.cn/gtwgsrnyan.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.andypj.xyz/gtbjlzeyov.html

[T25] Swift：结构体
来源：http://hz.yj202588.top/gtuukplzgt.html

struct P { var x: Int }
来源：http://hz.aibaodan.cn/gtqvxsowyv.html

[T26] Swift：类与重写
来源：http://hz.nanxuanxn.top/gtodwugvvc.html

class A: Base { override func f() {} }
来源：http://hz.yueranfly.top/gtyjeonkmg.html

[T27] Swift：错误处理
来源：http://hz.zhongyouzk.top/gtkneoqpex.html

do { try f() } catch { print(error) }
来源：http://hz.shanyushiyangkeji.top/gtoteptnfk.html

[T28] Swift：枚举
来源：http://hz.hysaishi.cn/gtezeoildj.html

enum Color { case red, green }
来源：http://hz.yuxming.cn/gtypubpgev.html

[T29] Swift：guard 提前返回
来源：http://hz.xuanzx.com/gtztevldyv.html

guard let x = opt else { return }
来源：http://hz.jyoumei.cn/gtylxwreus.html

[T30] Swift：协议
来源：http://hz.jqgufenzy.top/gtolykcqty.html

protocol Shape { func area() -> Double }
来源：http://hz.wangdashe.top/gtakusacom.html

[T31] Lua：Hello World
来源：http://hz.ivvv.top/gtedstclcm.html

print("Hello")
来源：http://hz.sysykeji.top/gtpaavlsbe.html

[T32] Lua：局部变量
来源：http://hz.jinqigfzy.top/gttlzvqbul.html

local a = 1
来源：http://hz.sxryk.cn/gtkgccdkmz.html

[T33] Lua：表（数组）
来源：http://hz.redwolf501.top/gtjkfygykr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hywenlv.cn/gtttstaawa.html

[T34] Lua：遍历表
来源：http://hz.hnqzz.top/gtwbbkszzk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinghuilouyu.cn/gtgdfatnvb.html

[T35] Lua：字典表
来源：http://hz.jianghu66.top/gtkgnnrvws.html

local d = { a = 1 };  d.b = 2
来源：http://hz.wangdashe.top/gtrysdctde.html

[T36] Lua：函数
来源：http://hz.kuanghao11.cn/gtgesfnhlh.html

function add(a, b) return a + b end
来源：http://hz.c1oappe.top/gtzfskgoax.html

[T37] Lua：字符串拼接
来源：http://hz.yj202588.top/gtzngcmpab.html

"a" .. "b"
来源：http://hz.sxryk.cn/gtxabnttes.html

[T38] Lua：条件
来源：http://hz.cheryme.top/gtdpfcwvsl.html

if x > 0 then print("正") end
来源：http://hz.tian-w.cn/gtrcaittmq.html

[T39] Lua：模式匹配
来源：http://hz.shanyushiyangtech.top/gtpfepsowp.html

string.find(s, "%d+")
来源：http://hz.aizwys.cn/gtfwlrnwfr.html

[T40] Lua：元表
来源：http://hz.ehwqpu.com/gtmgxbthql.html

setmetatable({}, { __index = base })
来源：http://hz.bjfxy.top/gtiwscdkcj.html

[T41] Perl：Hello World
来源：http://hz.wangdashe.top/gtxljtwmqd.html

print "Hello\n";
来源：http://hz.ydzc1.top/gtjtukqpvl.html

[T42] Perl：变量类型
来源：http://hz.jlsjyb.cn/gtegtbkfek.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.bjfxy.top/gtpjirdusw.html

[T43] Perl：字符串插值
来源：http://hz.xziqi.cn/gtackqxqgu.html

"值: $a"
来源：http://hz.nwbrower.top/gtdzijgcwe.html

[T44] Perl：条件
来源：http://hz.wangshuangyany.cn/gteejdagkf.html

if ($a > 0) { print "正"; }
来源：http://hz.yvedp.cn/gttalstluh.html

[T45] Perl：数组遍历
来源：http://hz.gotoacloud.top/gtcqzxlmfw.html

for my $x (@arr) { print $x; }
来源：http://hz.cashguo.top/gtdspmhvoq.html

[T46] Perl：哈希操作
来源：http://hz.aizwys.cn/gtozawaucj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hongshengwenyu.top/gtoeoxbxfb.html

[T47] Perl：正则捕获
来源：http://hz.sweek.top/gtbvtgdjja.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ybcxt.top/gtjfldipoc.html

[T48] Perl：正则替换
来源：http://hz.yanxiufei.cn/gtvcmjzlor.html

$s =~ s/old/new/g;
来源：http://hz.yvedp.cn/gtbngrptuh.html

[T49] Perl：函数
来源：http://hz.hnxiangtu.top/gtqmpkfcyn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hysaishi.cn/gtmaqdfguj.html

[T50] Perl：逐行读文件
来源：http://hz.pycfn.com/gtylyzrytg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.tianlin.xyz/gtrmrruqfs.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.wangshuangyany.cn/gtxkstiqtg.html

[T51] Scala：Hello World
来源：http://hz.yj20258.top/gtxbcwffla.html

println("Hello")
来源：http://hz.shangyingyoupin.top/gtgjbhkikm.html

[T52] Scala：变量
来源：http://hz.meibo888.top/gtqdpzdmnb.html

val a = 1;  var b = 2
来源：http://hz.yj20258.top/gtciwqjivi.html

[T53] Scala：字符串插值
来源：http://hz.hfpthk.cn/gttksykrlx.html

s"值: $b"
来源：http://hz.jqgufenzy.top/gtuqxlzewx.html

[T54] Scala：集合映射
来源：http://hz.feifeiyinyue.top/gtboyohhnk.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yvedp.cn/gthcqfutbn.html

[T55] Scala：集合过滤
来源：http://hz.guannengcc.top/gtjpjuvvej.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.c1oappe.top/gtfoexnlep.html

[T56] Scala：样例类
来源：http://hz.hammf.cn/gtoemabhsy.html

case class User(name: String, age: Int)
来源：http://hz.sufxvd.cn/gtuxrcuapb.html

[T57] Scala：模式匹配
来源：http://hz.shzxlz.cn/gtkqqhzjrr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.gaohongyu789.top/gtdsslhpsi.html

[T58] Scala：函数定义
来源：http://hz.guannengcc.top/gtvnyjeutb.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hfpthk.cn/gtplwlgzbb.html

[T59] Scala：循环
来源：http://hz.zycfv.cn/gteuysltja.html

for (i <- 1 to 10) println(i)
来源：http://hz.yuanzhike.top/gtkoccqtes.html

[T60] Scala：折叠
来源：http://hz.jianghu66.top/gtdgrephia.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.dianchejie.cn/gtmryvwcuz.html

================================================================================
来源：http://hz.yonumen.top/gtgxmwufhy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hammf.cn/gtrkwcjcat.html

================================================================================
来源：http://hz.chenlongwang.top/gtqolvbaht.html

[U01] Py：创建虚拟环境
来源：http://hz.cucudq.cn/gtvhskbjls.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hongshengwenyu.top/gtdffdjmpc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.feifeiyinyue.top/gtguxnheup.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinqigfzy.top/gtilbyzzlf.html

[U03] Py：加载 .env 配置
来源：http://hz.zhijiandao.cn/gtrlnlmqmi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jianghu66.top/gtyfklvkpw.html

[U04] Py：变量调试打印
来源：http://hz.shuidangran.top/gtputidpwf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ywan-chungtsiang.top/gtvydskhth.html

[U05] Py：列表去重且保序
来源：http://hz.andypj.xyz/gtpewighkd.html

list(dict.fromkeys(arr))
来源：http://hz.haohaochexian.top/gtqzegnbvb.html

[U06] Py：合并两个字典
来源：http://hz.jiagoushi.top/gtzqaraubr.html

{**a, **b}
来源：http://hz.yvedp.cn/gtviejzimv.html

[U07] Py：反转字典键值
来源：http://hz.feifeiyinyue.top/gtrmigmtxa.html

{v: k for k, v in d.items()}
来源：http://hz.zdqjudy.top/gtfozcxgti.html

[U08] Py：展平二维列表
来源：http://hz.0kj1m.cn/gtudfffelg.html

[y for x in nested for y in x]
来源：http://hz.jinqigufen.top/gtirzvlegt.html

[U09] Py：字典取最大值的键
来源：http://hz.hnqzz.top/gtkhalgevm.html

max(d, key=d.get)
来源：http://hz.sysykeji.top/gtxrumwlik.html

[U10] Py：按值排序字典
来源：http://hz.nanxinkj.top/gtcsbbcite.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.haohaochexian.top/gtqonzebut.html

[U11] Py：生成器表达式
来源：http://hz.ywan-chungtsiang.top/gtjvujeekl.html

(x * 2 for x in arr)
来源：http://hz.zhaomingkeji.xyz/gtscgfrjsi.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.dianchejie.cn/gtqboiqupt.html

Counter(arr).most_common(3)
来源：http://hz.feifeiyinyue.top/gtaufvqzne.html

[U13] Py：固定长度队列
来源：http://hz.jlsjyb.cn/gtgmyocsia.html

deque(maxlen=10)
来源：http://hz.zhengqikj.top/gtvomeespp.html

[U14] Py：分组收集到列表
来源：http://hz.shzxlz.cn/gtwolbnqff.html

defaultdict(list)
来源：http://hz.kuanghao11.cn/gtgaglgcrd.html

[U15] Py：高精度计时
来源：http://hz.316326.xyz/gtqdvpxclt.html

t = time.perf_counter()
来源：http://hz.jlsjyb.cn/gtuqunxvge.html

[U16] Py：命令行参数解析
来源：http://hz.hnxiangtu.top/gtbrnflcya.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ywan-chungtsiang.top/gtqdaovdhc.html

[U17] Py：初始化日志
来源：http://hz.sufxvd.cn/gtbbtbnkav.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.daxiang520.top/gtaccwvnlp.html

[U18] Py：预编译正则
来源：http://hz.chenzaomai.com/gtkezelrvd.html

pat = re.compile(r"\d+")
来源：http://hz.xuetiantiany.cn/gtszjtstuu.html

[U19] Py：正则替换带回调
来源：http://hz.jiagoushi.top/gthodjitcx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.quarkkingdee.top/gtfwyjortf.html

[U20] Py：缓存函数结果
来源：http://hz.fengsongda.top/gtqkzvjpae.html

@functools.lru_cache(maxsize=None)
来源：http://hz.smart0.xyz/gtaanpejku.html

[U21] Py：自定义上下文管理器
来源：http://hz.ywan-chungtsiang.top/gttvxvpzvi.html

@contextlib.contextmanager
来源：http://hz.dianchejie.cn/gtjvxoplge.html

[U22] Py：矩阵转置
来源：http://hz.yonumen.top/gtjfxpoqsw.html

list(zip(*m))
来源：http://hz.redwolf501.top/gtanlovgct.html

[U23] Py：分块读取大文件
来源：http://hz.gogol.net.cn/gtkicikbdi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.sufxvd.cn/gtknmdhtsr.html

[U24] Py：路径操作
来源：http://hz.zhoulong.xyz/gtajsirtrt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gogol.net.cn/gtvmuxqcph.html

[U25] Py：CSV 按字典读
来源：http://hz.hywenlv.cn/gthgkxegkl.html

csv.DictReader(f)
来源：http://hz.daxiang520.top/gtqbprrzxr.html

[U26] Py：并发下载
来源：http://hz.jianghu66.top/gtukahppcz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.fengsongda.top/gtwogjwbtb.html

[U27] Py：异步 HTTP
来源：http://hz.cashguo.top/gtmozfhoff.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.kuanghao11.cn/gtnfeczjaj.html

[U28] Py：类型别名
来源：http://hz.ydzc1.top/gttyohgqac.html

UserId = int
来源：http://hz.aizwys.cn/gtcxzlbbve.html

[U29] Py：属性校验
来源：http://hz.316326.xyz/gtdehxcziv.html

@property 与 @x.setter 配合
来源：http://hz.ppjwa.cn/gtepidwfuz.html

[U30] Py：数据类
来源：http://hz.yangfankeji.com/gtgymxcgid.html

@dataclass(slots=True)
来源：http://hz.kuanghao11.cn/gteikcckdh.html

[U31] Py：单测
来源：http://hz.ehwqpu.com/gtnphbdqzl.html

python -m pytest -q
来源：http://hz.gaohongyu789.top/gticoikqti.html

[U32] Py：代码格式化
来源：http://hz.zhengqikj.top/gtqrhiriul.html

ruff format . && ruff check --fix .
来源：http://hz.jiagoushi.top/gtpjwvrzzv.html

[U33] Py：打包发布
来源：http://hz.xziqi.cn/gtiwfmeytg.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.316326.xyz/gtmzgmkhqw.html

[U34] Py：判断编码
来源：http://hz.gogol.net.cn/gtowdzfgre.html

chardet.detect(raw)
来源：http://hz.gogol.net.cn/gtncomysgo.html

[U35] Py：发送邮件
来源：http://hz.ywan-chungtsiang.top/gtedpjqzio.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zdqjudy.top/gtwazmmist.html

[U36] Py：定时任务
来源：http://hz.haohaochexian.top/gtlhxggigj.html

schedule.every(10).minutes.do(job)
来源：http://hz.yj20258.top/gttcnhmzcf.html

[U37] Py：读写 Excel
来源：http://hz.hywenlv.cn/gtezdehijz.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.chenzaomai.com/gtkmgzozfi.html

[U38] Py：获取脚本所在目录
来源：http://hz.fengsongda.top/gtvljckxbq.html

Path(__file__).resolve().parent
来源：http://hz.nanxuanxn.top/gtqnhokzze.html

[U39] Py：判断是否在交互环境
来源：http://hz.haohaochexian.top/gtegxpedzf.html

sys.stdout.isatty()
来源：http://hz.jianghu66.top/gtosctjxrr.html

[U40] Py：打印到标准错误
来源：http://hz.jlsjyb.cn/gtanbeilxe.html

print("err", file=sys.stderr)
来源：http://hz.yj20258.top/gtknwjfqad.html


<!-- 参考信息 -->