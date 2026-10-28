代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://hz.xziqi.cn/gtlorvkkfr.html

[S15] C：类型转换
来源：http://hz.yonumen.top/gtkywgtcqg.html

(double) a / b
来源：http://hz.yuxming.cn/gtuhzrrmcf.html

[S16] C：位操作置位
来源：http://hz.zycfv.cn/gtijmjeetk.html

x |= (1 << 3);
来源：http://hz.hysaishi.cn/gtlbfpxwfd.html

[S17] C：安全拼接字符串
来源：http://hz.quarkkingdee.top/gtxyhmbdgs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gaohongyu789.top/gtsysiqzyn.html

[S18] C：命令行参数
来源：http://hz.zhaomingkeji.xyz/gtgdqkqqge.html

int main(int argc, char **argv)
来源：http://hz.svipenyu.cn/gttcaqtmre.html

[S19] C：快速排序
来源：http://hz.shanyushiyangtech.top/gtiadwpdyh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yj20258.top/gtoewyezfu.html

[S20] C：二分查找
来源：http://hz.nanxinkj.top/gthjwnuouy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.vqdsnc.cn/gtrtmyvyzz.html

[S21] C：字符类别判断
来源：http://hz.shzxlz.cn/gthvlvkpnj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhixingplan.top/gtwuiqmhru.html

[S22] C：字符串转数字
来源：http://hz.havefunace.top/gtuopktysx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hammf.cn/gtcawvkhzd.html

[S23] C：随机数
来源：http://hz.dianchejie.cn/gtiibxefra.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.pycfn.com/gtbstjwqmm.html

[S24] C：获取本地时间
来源：http://hz.yonumen.top/gtacrkssgw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.aibaodan.cn/gtjiwxeawv.html

[S25] C：内存拷贝
来源：http://hz.jianghu66.top/gtrnfuyvfz.html

memcpy(dst, src, n);
来源：http://hz.bjfxy.top/gtcnwncghj.html

[S26] C：内存清零
来源：http://hz.chenzaomai.com/gttplzgjbh.html

memset(a, 0, sizeof a);
来源：http://hz.9152youxi.cn/gtvbthaeui.html

[S27] C：定义常量
来源：http://hz.hywenlv.cn/gtdyacvunj.html

const double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtdkmgyror.html

[S28] C：静态变量
来源：http://hz.ehwqpu.com/gtgfxqzrrn.html

static int counter = 0;
来源：http://hz.pengpengdd.cyou/gtpeglhgmr.html

[S29] C：变参函数
来源：http://hz.dashuyun.cn/gttzsyquyd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinqigufen.top/gtlwjpfomq.html

[S30] C：头文件保护
来源：http://hz.havefunace.top/gtzayeavhh.html

#ifndef X_H
来源：http://hz.52xcode.cn/gtbcbkzxuo.html

#define X_H
来源：http://hz.jqgfzy.top/gtpmwexfte.html

#endif
来源：http://hz.yangfankeji.com/gtbehswqbd.html

[S31] C++：Hello World
来源：http://hz.ivvv.top/gtjizqlhtq.html

#include <iostream>
来源：http://hz.shuidangran.top/gtkdgemesn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ivvv.top/gttturbwgw.html

[S32] C++：字符串
来源：http://hz.cheryme.top/gtzeqqxvjj.html

std::string s = "hi";  s += "!";
来源：http://hz.yuanzhike.top/gtvkpfuwif.html

[S33] C++：vector 增删
来源：http://hz.hammf.cn/gtdrhhgvei.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.cqqwz.cn/gtezuizxpz.html

[S34] C++：遍历 vector
来源：http://hz.gotoacloud.top/gtxrmqmead.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.vqdsnc.cn/gtlwzojdox.html

[S35] C++：map
来源：http://hz.yj20258888.top/gtxjbillbp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.svipenyu.cn/gtaboohpdk.html

[S36] C++：unordered_map
来源：http://hz.nwbrower.top/gtmlqxwknt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hfpthk.cn/gthpytkieh.html

[S37] C++：set
来源：http://hz.fengsongda.top/gtxomkrgfi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jianghu66.top/gttwxwiaae.html

[S38] C++：排序
来源：http://hz.wangdashe.top/gtsgrchzec.html

std::sort(v.begin(), v.end());
来源：http://hz.cucudq.cn/gtfewiwoss.html

[S39] C++：自定义比较器排序
来源：http://hz.cucudq.cn/gtywcviqlp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.smart0.xyz/gtrqjraqdr.html

[S40] C++：查找元素
来源：http://hz.ydjk.org.cn/gtwelimlfw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yanxiufei.cn/gtrmueleyd.html

[S41] C++：类与构造函数
来源：http://hz.yj20258888.top/gtijlvrdgx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.kuanghao11.cn/gtvwpyfbxw.html

[S42] C++：继承与虚函数
来源：http://hz.316326.xyz/gtwjozzvps.html

class B : public Base { public: void f() override {} };
来源：http://hz.xinyue.icu/gtuhqksszu.html

[S43] C++：智能指针
来源：http://hz.chenlongwang.top/gtmlmkmtan.html

auto p = std::make_unique<int>(5);
来源：http://hz.ybcxt.top/gtkscmrmqb.html

[S44] C++：引用传参
来源：http://hz.nanxinkj.top/gtglqwhyiy.html

void inc(int &x) { ++x; }
来源：http://hz.xinyue.icu/gtvlgiprqh.html

[S45] C++：lambda
来源：http://hz.zhijiandao.cn/gtqeurhhxq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sxryk.cn/gtsizupnnd.html

[S46] C++：函数模板
来源：http://hz.meibo888.top/gtkvvqhnak.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj202588.top/gtxociucmq.html

[S47] C++：结构化绑定遍历
来源：http://hz.shuidangran.top/gthbasatfm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.guowangkeji.top/gtubdpyqtn.html

[S48] C++：逐行读文件
来源：http://hz.quarkkingdee.top/gtxcninpey.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ehwqpu.com/gtqvzvcgwl.html

while (std::getline(in, line)) { }
来源：http://hz.cashguo.top/gtnhxbkbla.html

[S49] C++：写文件
来源：http://hz.sufxvd.cn/gteaujygvn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tanke756.top/gtegkubxxq.html

[S50] C++：格式化数字
来源：http://hz.xuetiantiany.cn/gtdibwimjr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shzxlz.cn/gtesurxwwr.html

[S51] C++：显式类型转换
来源：http://hz.9152youxi.cn/gtyalobvra.html

static_cast<double>(a) / b
来源：http://hz.nanxuanxn.top/gticllhbqc.html

[S52] C++：const 与 noexcept
来源：http://hz.shangyingyoupin.top/gtlemzlnlm.html

int size() const noexcept { return n_; }
来源：http://hz.gotoacloud.top/gtckqiidka.html

[S53] C++：移动语义
来源：http://hz.birdmap.top/gtxtyooemx.html

std::vector<int> w = std::move(v);
来源：http://hz.yangfankeji.com/gtctrcjzam.html

[S54] C++：异常处理
来源：http://hz.pengpengdd.cyou/gttlfhjamf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xinyue.icu/gtetlklolo.html

[S55] C++：结构化绑定
来源：http://hz.shanyushiyangtech.top/gtjwtjkugu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xuanzx.com/gtcistwcfj.html

[S56] C++：optional
来源：http://hz.aizwys.cn/gtmvzncjwd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.pengpengdd.cyou/gtrantvkqm.html

[S57] C++：编译期常量
来源：http://hz.zhengqikj.top/gtrkydvgja.html

constexpr int N = 10;
来源：http://hz.smart0.xyz/gtkodbcdoq.html

[S58] C++：命名空间
来源：http://hz.zhengqikj.top/gtmuwslwrk.html

namespace ns { int f() { return 1; } }
来源：http://hz.ywan-chungtsiang.top/gtcmpikhux.html

[S59] C++：静态断言
来源：http://hz.yonumen.top/gtuccmjnuc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sysykeji.top/gtabsyybky.html

[S60] C++：遍历并删除元素
来源：http://hz.pengpengdd.cyou/gtiufdnuxk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jiagoushi.top/gtuyyosufl.html

================================================================================
来源：http://hz.xinyue.icu/gtnxrkkwxb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj20258.top/gtfwlbxztl.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtwhwpzfna.html

[T01] Kotlin：Hello World
来源：http://hz.feifeiyinyue.top/gteflxvnjl.html

println("Hello")
来源：http://hz.dashuyun.cn/gtdlpucgau.html

[T02] Kotlin：变量
来源：http://hz.yongpay.top/gtixgdvwmg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.daxiang520.top/gtpqiilqyg.html

[T03] Kotlin：字符串模板
来源：http://hz.gogol.net.cn/gtjouqlnqs.html

"值: $b"
来源：http://hz.jyoumei.cn/gtxhnvzbzu.html

[T04] Kotlin：空安全
来源：http://hz.xuanzx.com/gtljgivsid.html

val n: String? = null;  n?.length
来源：http://hz.hnxiangtu.top/gtkfilvrtv.html

[T05] Kotlin：when 表达式
来源：http://hz.yanxiufei.cn/gtrfzkrgjw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinqigfzy.top/gtyzexlmqa.html

[T06] Kotlin：集合映射
来源：http://hz.hammf.cn/gtxmoiitbq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.mhx1999.top/gtzfwdaeja.html

[T07] Kotlin：集合过滤
来源：http://hz.daxiang520.top/gtmljuvmbp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.pengpengdd.cyou/gtyzodxgnq.html

[T08] Kotlin：数据类
来源：http://hz.sysykeji.top/gtpihzumlr.html

data class User(val name: String, val age: Int)
来源：http://hz.xylfe.cn/gtiupjwwah.html

[T09] Kotlin：扩展函数
来源：http://hz.jianghu66.top/gtjandvfmo.html

fun String.exclaim() = this + "!"
来源：http://hz.shzxlz.cn/gtlqxatwaf.html

[T10] Kotlin：默认参数
来源：http://hz.svipenyu.cn/gtlrldcrhe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ehwqpu.com/gtuspejqep.html

[T11] Kotlin：协程
来源：http://hz.xuetiantiany.cn/gtovofzjpb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.wangshuangyany.cn/gtyenmkmxg.html

[T12] Kotlin：解构声明
来源：http://hz.jqgfzy.top/gtmzflokej.html

val (a, b) = Pair(1, 2)
来源：http://hz.sweek.top/gtygigopom.html

[T13] Kotlin：只读 Map
来源：http://hz.yueranfly.top/gtcgvozpqm.html

val m = mapOf("a" to 1)
来源：http://hz.dashuyun.cn/gtpcpdzsub.html

[T14] Kotlin：循环
来源：http://hz.cdnleiting.top/gtkmnbkxpv.html

for (i in 1..10) println(i)
来源：http://hz.ppjwa.cn/gtdcglkfeh.html

[T15] Kotlin：接口
来源：http://hz.jlsjyb.cn/gtetwpddiy.html

interface Shape { fun area(): Double }
来源：http://hz.jqgufenzy.top/gttbbjedwx.html

[T16] Swift：Hello World
来源：http://hz.ydzc1.top/gtyvvsroeh.html

print("Hello")
来源：http://hz.yanxiufei.cn/gtaghirwas.html

[T17] Swift：变量与常量
来源：http://hz.gotoacloud.top/gtyvrkmsho.html

var a = 1;  let b = 2
来源：http://hz.hfpthk.cn/gtjjdzehyy.html

[T18] Swift：字符串插值
来源：http://hz.shangyingyoupin.top/gtccgfjtin.html

"值: \(b)"
来源：http://hz.xinyue.icu/gtdfvbxzhs.html

[T19] Swift：可选绑定
来源：http://hz.meibo888.top/gtcidxvjsk.html

if let n = opt { print(n) }
来源：http://hz.gotoacloud.top/gtpgrrdqst.html

[T20] Swift：数组操作
来源：http://hz.jianghu66.top/gtrtdeahos.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cucudq.cn/gtqzllizvg.html

[T21] Swift：遍历
来源：http://hz.yuxming.cn/gtuwuaujaq.html

for x in a { print(x) }
来源：http://hz.chenjidiqi.icu/gtrygbkbtm.html

[T22] Swift：字典
来源：http://hz.shuidangran.top/gtzxyrfvii.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xuetiantiany.cn/gttaairwjo.html

[T23] Swift：函数
来源：http://hz.meibo888.top/gtxzmofrus.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yj20258.top/gttbyoahla.html

[T24] Swift：闭包
来源：http://hz.jinqigufen.top/gtcvirzzlh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.iojbl.cn/gtlpkkpvmn.html

[T25] Swift：结构体
来源：http://hz.svipenyu.cn/gtnzakqlhr.html

struct P { var x: Int }
来源：http://hz.ppjwa.cn/gtquziqotj.html

[T26] Swift：类与重写
来源：http://hz.yuanzhike.top/gtlitwqhjg.html

class A: Base { override func f() {} }
来源：http://hz.dianchejie.cn/gtqztuvdzn.html

[T27] Swift：错误处理
来源：http://hz.cucudq.cn/gtsgzhytlg.html

do { try f() } catch { print(error) }
来源：http://hz.gogol.net.cn/gtfxgybpvt.html

[T28] Swift：枚举
来源：http://hz.zhaomingkeji.xyz/gttnfdkmof.html

enum Color { case red, green }
来源：http://hz.cqqwz.cn/gtwdgnweuz.html

[T29] Swift：guard 提前返回
来源：http://hz.ivvv.top/gtbydxguqc.html

guard let x = opt else { return }
来源：http://hz.9152youxi.cn/gtqwdypzke.html

[T30] Swift：协议
来源：http://hz.shanyushiyangtech.top/gtmwnwhjol.html

protocol Shape { func area() -> Double }
来源：http://hz.nanxuanxn.top/gtxbnbgvfx.html

[T31] Lua：Hello World
来源：http://hz.zhongyouzk.top/gttvzwlbwf.html

print("Hello")
来源：http://hz.cheryme.top/gtdqzmbnho.html

[T32] Lua：局部变量
来源：http://hz.zycfv.cn/gtppfeoafn.html

local a = 1
来源：http://hz.sxryk.cn/gtlmmokpfl.html

[T33] Lua：表（数组）
来源：http://hz.xinyue.icu/gthnbuexfc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.tanke756.top/gtwpodfdvh.html

[T34] Lua：遍历表
来源：http://hz.zhijiandao.cn/gtndxytycm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ppjwa.cn/gtktpedwtk.html

[T35] Lua：字典表
来源：http://hz.xinyue.icu/gtmzygtwqv.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yonumen.top/gtlmurevtt.html

[T36] Lua：函数
来源：http://hz.ydzc1.top/gtqigfzpyo.html

function add(a, b) return a + b end
来源：http://hz.316326.xyz/gtswdblhab.html

[T37] Lua：字符串拼接
来源：http://hz.meibo888.top/gtzfwriqkf.html

"a" .. "b"
来源：http://hz.c1oappe.top/gtounneanh.html

[T38] Lua：条件
来源：http://hz.yj20258888.top/gtpkzrnwdo.html

if x > 0 then print("正") end
来源：http://hz.316326.xyz/gtzzowtwkw.html

[T39] Lua：模式匹配
来源：http://hz.mhx1999.top/gtgzibzfhj.html

string.find(s, "%d+")
来源：http://hz.jinyuanbaomall.cn/gtlryrqeqz.html

[T40] Lua：元表
来源：http://hz.ydjk.org.cn/gttijstqpo.html

setmetatable({}, { __index = base })
来源：http://hz.jqgfzy.top/gtmdnwhyae.html

[T41] Perl：Hello World
来源：http://hz.0kj1m.cn/gtamtufuxb.html

print "Hello\n";
来源：http://hz.andypj.xyz/gtxczxbnfx.html

[T42] Perl：变量类型
来源：http://hz.nanxuanxn.top/gtchlzirgz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gotoacloud.top/gtdipavhdo.html

[T43] Perl：字符串插值
来源：http://hz.9152youxi.cn/gtxxghntrr.html

"值: $a"
来源：http://hz.tanke756.top/gtusdomgvf.html

[T44] Perl：条件
来源：http://hz.aibaodan.cn/gtgylssyqy.html

if ($a > 0) { print "正"; }
来源：http://hz.gogol.net.cn/gtxbniijba.html

[T45] Perl：数组遍历
来源：http://hz.snrcjt.cn/gtubtynaok.html

for my $x (@arr) { print $x; }
来源：http://hz.jqgfzy.top/gthggabmql.html

[T46] Perl：哈希操作
来源：http://hz.zhoulong.xyz/gtgbfobjjv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.birdmap.top/gtrqbgdebu.html

[T47] Perl：正则捕获
来源：http://hz.cqqwz.cn/gtvvvhymwp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhixingplan.top/gtkrptcuty.html

[T48] Perl：正则替换
来源：http://hz.meibo888.top/gtizfibtdf.html

$s =~ s/old/new/g;
来源：http://hz.cheryme.top/gtewwlrmry.html

[T49] Perl：函数
来源：http://hz.zdqjudy.top/gtpltriglb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cucudq.cn/gtxhokhxlb.html

[T50] Perl：逐行读文件
来源：http://hz.chenzaomai.com/gtpqaalfdr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sysykeji.top/gttjqvwrvr.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.wangdashe.top/gtmncjowdb.html

[T51] Scala：Hello World
来源：http://hz.xuetiantiany.cn/gtbqslztxq.html

println("Hello")
来源：http://hz.chenlongwang.top/gtjesfwwxk.html

[T52] Scala：变量
来源：http://hz.dashuyun.cn/gtttumruum.html

val a = 1;  var b = 2
来源：http://hz.wangshuangyany.cn/gttrepglri.html

[T53] Scala：字符串插值
来源：http://hz.sufxvd.cn/gtbzjnomkn.html

s"值: $b"
来源：http://hz.cucudq.cn/gtlksaastd.html

[T54] Scala：集合映射
来源：http://hz.9152youxi.cn/gthplvgsau.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.sysykeji.top/gtevxswcoz.html

[T55] Scala：集合过滤
来源：http://hz.ydjk.org.cn/gthprenlof.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhoulong.xyz/gthslejbug.html

[T56] Scala：样例类
来源：http://hz.cashguo.top/gtplsvkxsg.html

case class User(name: String, age: Int)
来源：http://hz.snrcjt.cn/gtreocyggl.html

[T57] Scala：模式匹配
来源：http://hz.hnqzz.top/gtcodqdihy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zdqjudy.top/gtfgbnitti.html

[T58] Scala：函数定义
来源：http://hz.gotoacloud.top/gttfuegxji.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jqgufenzy.top/gtdwznwqpw.html

[T59] Scala：循环
来源：http://hz.haohaochexian.top/gtqvliwoos.html

for (i <- 1 to 10) println(i)
来源：http://hz.sufxvd.cn/gtyvxvkfjj.html

[T60] Scala：折叠
来源：http://hz.yuxming.cn/gtfyihvenh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.aizwys.cn/gtgwgyjqhw.html

================================================================================
来源：http://hz.9152youxi.cn/gtmrrpghyn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ydzc1.top/gtkyeojezm.html

================================================================================
来源：http://hz.vqdsnc.cn/gtvsvramjc.html

[U01] Py：创建虚拟环境
来源：http://hz.hysaishi.cn/gtvgzptbey.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jqgfzy.top/gtspdxevtj.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jinqigfzy.top/gtxfmultvp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ywan-chungtsiang.top/gtsyqacrle.html

[U03] Py：加载 .env 配置
来源：http://hz.shangyingyoupin.top/gtuofkwnvx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.gotoacloud.top/gtwuqxeozm.html

[U04] Py：变量调试打印
来源：http://hz.yj202588.top/gtnyvglvfd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.vqdsnc.cn/gttsbbckuw.html

[U05] Py：列表去重且保序
来源：http://hz.pengpengdd.cyou/gtebnwqqyd.html

list(dict.fromkeys(arr))
来源：http://hz.jqgfzy.top/gtutioushd.html

[U06] Py：合并两个字典
来源：http://hz.jyoumei.cn/gtrzfdcqng.html

{**a, **b}
来源：http://hz.mhx1999.top/gtuotjyknd.html

[U07] Py：反转字典键值
来源：http://hz.316326.xyz/gttkdsfjoh.html

{v: k for k, v in d.items()}
来源：http://hz.xylfe.cn/gthmruhifc.html

[U08] Py：展平二维列表
来源：http://hz.dashuyun.cn/gtkmofjvlz.html

[y for x in nested for y in x]
来源：http://hz.jyoumei.cn/gtwdlqzuwu.html

[U09] Py：字典取最大值的键
来源：http://hz.feifeiyinyue.top/gthzwzjqbx.html

max(d, key=d.get)
来源：http://hz.xinyue.icu/gtqcrgsbew.html

[U10] Py：按值排序字典
来源：http://hz.iojbl.cn/gtjtfcsfin.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ehwqpu.com/gtcrhkpukr.html

[U11] Py：生成器表达式
来源：http://hz.daria6918.cn/gtrkuyambw.html

(x * 2 for x in arr)
来源：http://hz.ydzc1.top/gthrvozhnc.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hongshengwenyu.top/gtzyuuyekv.html

Counter(arr).most_common(3)
来源：http://hz.nanxinkj.top/gtkfsuxucj.html

[U13] Py：固定长度队列
来源：http://hz.xuanzx.com/gtmhgimcpc.html

deque(maxlen=10)
来源：http://hz.feifeiyinyue.top/gtiwzxwpel.html

[U14] Py：分组收集到列表
来源：http://hz.jianghu66.top/gtxjfxnmvi.html

defaultdict(list)
来源：http://hz.redwolf501.top/gtzboqrakr.html

[U15] Py：高精度计时
来源：http://hz.ehwqpu.com/gtbzcwpkaq.html

t = time.perf_counter()
来源：http://hz.ybcxt.top/gtuvrfqfjx.html

[U16] Py：命令行参数解析
来源：http://hz.sufxvd.cn/gtavkmzrhf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinghuilouyu.cn/gtxgiaswhz.html

[U17] Py：初始化日志
来源：http://hz.hfpthk.cn/gtvowfxepi.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.iojbl.cn/gtlzedpqst.html

[U18] Py：预编译正则
来源：http://hz.zhixingplan.top/gthvrrvylr.html

pat = re.compile(r"\d+")
来源：http://hz.tanke756.top/gtixnrjtix.html

[U19] Py：正则替换带回调
来源：http://hz.xuanzx.com/gthrcvtitz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.mhx1999.top/gtcgzdjtck.html

[U20] Py：缓存函数结果
来源：http://hz.jianghu66.top/gtwhnjcxxj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.0kj1m.cn/gtekggxkzl.html

[U21] Py：自定义上下文管理器
来源：http://hz.9152youxi.cn/gtclegkvxa.html

@contextlib.contextmanager
来源：http://hz.hnqzz.top/gtatlszade.html

[U22] Py：矩阵转置
来源：http://hz.gogol.net.cn/gtvstdffna.html

list(zip(*m))
来源：http://hz.yj20258888.top/gttrcqnbxx.html

[U23] Py：分块读取大文件
来源：http://hz.jqgfzy.top/gticreyljw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yueranfly.top/gtuhvwnbjx.html

[U24] Py：路径操作
来源：http://hz.sufxvd.cn/gtqnitohnd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.iojbl.cn/gttbqargok.html

[U25] Py：CSV 按字典读
来源：http://hz.redwolf501.top/gtvbjsfwdi.html

csv.DictReader(f)
来源：http://hz.tianlin.xyz/gttekzwpqe.html

[U26] Py：并发下载
来源：http://hz.guowangkeji.top/gtgkbfmmks.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.52xcode.cn/gtuliuxqbg.html

[U27] Py：异步 HTTP
来源：http://hz.feifeiyinyue.top/gtmqkclgkz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.havefunace.top/gtiurtjqge.html

[U28] Py：类型别名
来源：http://hz.shangyingyoupin.top/gtxpnbjbgg.html

UserId = int
来源：http://hz.9152youxi.cn/gtqwnhclgg.html

[U29] Py：属性校验
来源：http://hz.ybcxt.top/gtmqpzakln.html

@property 与 @x.setter 配合
来源：http://hz.jqgfzy.top/gtogzgqibd.html

[U30] Py：数据类
来源：http://hz.meibo888.top/gtwkxnglqd.html

@dataclass(slots=True)
来源：http://hz.daria6918.cn/gthsobltst.html

[U31] Py：单测
来源：http://hz.jiagoushi.top/gtcedpqofj.html

python -m pytest -q
来源：http://hz.zhoulong.xyz/gthwbdbxho.html

[U32] Py：代码格式化
来源：http://hz.cdnleiting.top/gthvaapijm.html

ruff format . && ruff check --fix .
来源：http://hz.zhongyouzk.top/gtursgqcio.html

[U33] Py：打包发布
来源：http://hz.vqdsnc.cn/gtlcbpehmt.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hammf.cn/gtprsuuadg.html

[U34] Py：判断编码
来源：http://hz.snrcjt.cn/gtntuvoruo.html

chardet.detect(raw)
来源：http://hz.shanyushiyangtech.top/gtldmqrpye.html

[U35] Py：发送邮件
来源：http://hz.jinqigfzy.top/gtnunuinyh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yuxming.cn/gtmhmhtlaf.html

[U36] Py：定时任务
来源：http://hz.jlsjyb.cn/gtwdjzerku.html

schedule.every(10).minutes.do(job)
来源：http://hz.0kj1m.cn/gtvonyulis.html

[U37] Py：读写 Excel
来源：http://hz.smart0.xyz/gtiqbkbgjr.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.wangdashe.top/gtfkkxjyor.html

[U38] Py：获取脚本所在目录
来源：http://hz.jlsjyb.cn/gtlgmizulf.html

Path(__file__).resolve().parent
来源：http://hz.jinyuanbaomall.cn/gtiuhjrzil.html


<!-- 参考信息 -->