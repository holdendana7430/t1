代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.birdmap.top/gtobvepvjv.html

[S13] C：宏定义
来源：http://hz.xylfe.cn/gtpztqqgag.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ehwqpu.com/gtyveqhisv.html

[S14] C：枚举
来源：http://hz.zhijiandao.cn/gtyprnwioy.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.daxiang520.top/gtzvfggxjd.html

[S15] C：类型转换
来源：http://hz.mhx1999.top/gtllsnglol.html

(double) a / b
来源：http://hz.xylfe.cn/gttcpuiphl.html

[S16] C：位操作置位
来源：http://hz.meibo888.top/gtttemcbhs.html

x |= (1 << 3);
来源：http://hz.pycfn.com/gtgoosvhmk.html

[S17] C：安全拼接字符串
来源：http://hz.andypj.xyz/gtfilcuxow.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sysykeji.top/gtpwcealkr.html

[S18] C：命令行参数
来源：http://hz.zhijiandao.cn/gtvfgcvatv.html

int main(int argc, char **argv)
来源：http://hz.cheryme.top/gtyfxywlmi.html

[S19] C：快速排序
来源：http://hz.sxryk.cn/gtzmpzcbaz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nanxuanxn.top/gtrfwtuzqv.html

[S20] C：二分查找
来源：http://hz.mhx1999.top/gthlqkhoix.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ydjk.org.cn/gtogrxqxxc.html

[S21] C：字符类别判断
来源：http://hz.svipenyu.cn/gtegtbsudw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xuetiantiany.cn/gtmrthjeea.html

[S22] C：字符串转数字
来源：http://hz.zhiwuduotai.top/gtpratzrva.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhaomingkeji.xyz/gtpbpuiydh.html

[S23] C：随机数
来源：http://hz.redwolf501.top/gttsfhxknh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhiwuduotai.top/gtnonmejnm.html

[S24] C：获取本地时间
来源：http://hz.smart0.xyz/gtevilmwsp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinghuilouyu.cn/gtvkghevzh.html

[S25] C：内存拷贝
来源：http://hz.dashuyun.cn/gtfmfxxvwp.html

memcpy(dst, src, n);
来源：http://hz.zhijiandao.cn/gtnywnztpw.html

[S26] C：内存清零
来源：http://hz.sysykeji.top/gtcvpldvni.html

memset(a, 0, sizeof a);
来源：http://hz.birdmap.top/gtcxinqixa.html

[S27] C：定义常量
来源：http://hz.yueranfly.top/gtyhkehtkx.html

const double PI = 3.14159;
来源：http://hz.jqgfzy.top/gtqznemuml.html

[S28] C：静态变量
来源：http://hz.shanyushiyangtech.top/gtzcllbnot.html

static int counter = 0;
来源：http://hz.xylfe.cn/gtttulqoxk.html

[S29] C：变参函数
来源：http://hz.bjfxy.top/gtevdpskck.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zdqjudy.top/gtykfgnzgo.html

[S30] C：头文件保护
来源：http://hz.hnxiangtu.top/gtsitostvw.html

#ifndef X_H
来源：http://hz.shanyushiyangkeji.top/gtcwhqkeqf.html

#define X_H
来源：http://hz.cheryme.top/gtgqhvxkvz.html

#endif
来源：http://hz.iojbl.cn/gtughwqivf.html

[S31] C++：Hello World
来源：http://hz.guowangkeji.top/gtrxkymagv.html

#include <iostream>
来源：http://hz.yongpay.top/gtnapfzuty.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gaohongyu789.top/gtwruhnmvc.html

[S32] C++：字符串
来源：http://hz.yangfankeji.com/gttwehtxyw.html

std::string s = "hi";  s += "!";
来源：http://hz.shuidangran.top/gtvqfxwyqa.html

[S33] C++：vector 增删
来源：http://hz.zdqjudy.top/gtjjfbwghe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jinghuilouyu.cn/gtbfhdksfp.html

[S34] C++：遍历 vector
来源：http://hz.jinqigufen.top/gtmyulbgbn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.daria6918.cn/gtpdkywjqp.html

[S35] C++：map
来源：http://hz.yueranfly.top/gtdpefcrue.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhiwuduotai.top/gtizxhtwsw.html

[S36] C++：unordered_map
来源：http://hz.xuanzx.com/gtlpmpycyf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgufenzy.top/gtxffpiwds.html

[S37] C++：set
来源：http://hz.jinqigfzy.top/gtlunqildu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.pycfn.com/gtdajrqxxc.html

[S38] C++：排序
来源：http://hz.pengpengdd.cyou/gtxngxodvx.html

std::sort(v.begin(), v.end());
来源：http://hz.jlsjyb.cn/gtrpwexllz.html

[S39] C++：自定义比较器排序
来源：http://hz.redwolf501.top/gttkptefuy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinyuanbaomall.cn/gtklbtmihf.html

[S40] C++：查找元素
来源：http://hz.yj20258888.top/gtkiawaqgc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zycfv.cn/gtzqubitgs.html

[S41] C++：类与构造函数
来源：http://hz.ybcxt.top/gtailcjjct.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gaohongyu789.top/gtyhjpstkn.html

[S42] C++：继承与虚函数
来源：http://hz.zhijiandao.cn/gtxcwxijmr.html

class B : public Base { public: void f() override {} };
来源：http://hz.iojbl.cn/gtxdcjnunb.html

[S43] C++：智能指针
来源：http://hz.nanxinkj.top/gtgkyhzmuw.html

auto p = std::make_unique<int>(5);
来源：http://hz.sweek.top/gtildumnhl.html

[S44] C++：引用传参
来源：http://hz.mhx1999.top/gtfsaswvup.html

void inc(int &x) { ++x; }
来源：http://hz.jiagoushi.top/gtxblofyjw.html

[S45] C++：lambda
来源：http://hz.aibaodan.cn/gthydciocb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cashguo.top/gttedczjmv.html

[S46] C++：函数模板
来源：http://hz.xuanzx.com/gtmydkyepr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.vqdsnc.cn/gtlkxepxkd.html

[S47] C++：结构化绑定遍历
来源：http://hz.gzhubu.top/gtbpgwrkhj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.316326.xyz/gtwkbxlgzk.html

[S48] C++：逐行读文件
来源：http://hz.jqgfzy.top/gtsyjzrpdp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sysykeji.top/gtrthfkprw.html

while (std::getline(in, line)) { }
来源：http://hz.jlsjyb.cn/gtkzchollm.html

[S49] C++：写文件
来源：http://hz.yj20258888.top/gtugpzxrcv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.smart0.xyz/gtzrjmcdwe.html

[S50] C++：格式化数字
来源：http://hz.ydzc1.top/gtvabuhncx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yonumen.top/gtsvdgqooy.html

[S51] C++：显式类型转换
来源：http://hz.smart0.xyz/gtmpnteihv.html

static_cast<double>(a) / b
来源：http://hz.zhongyouzk.top/gtjaortfxy.html

[S52] C++：const 与 noexcept
来源：http://hz.hywenlv.cn/gtnadojxyf.html

int size() const noexcept { return n_; }
来源：http://hz.snrcjt.cn/gtrspnszpa.html

[S53] C++：移动语义
来源：http://hz.chenjidiqi.icu/gtmuwmzmgy.html

std::vector<int> w = std::move(v);
来源：http://hz.jqgfzy.top/gtkelgrmqv.html

[S54] C++：异常处理
来源：http://hz.zhixingplan.top/gtgomxxfvn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cdnleiting.top/gtldnnitjl.html

[S55] C++：结构化绑定
来源：http://hz.xinyue.icu/gtpybpadqw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhaomingkeji.xyz/gtzmejjcqm.html

[S56] C++：optional
来源：http://hz.zhiwuduotai.top/gtvalxoxyk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jinghuilouyu.cn/gtoxnljxso.html

[S57] C++：编译期常量
来源：http://hz.zhengqikj.top/gtmehddvsf.html

constexpr int N = 10;
来源：http://hz.zycfv.cn/gtnejjierq.html

[S58] C++：命名空间
来源：http://hz.zycfv.cn/gtfeddcfuo.html

namespace ns { int f() { return 1; } }
来源：http://hz.xziqi.cn/gtdgdewmtj.html

[S59] C++：静态断言
来源：http://hz.wangdashe.top/gthmurkeaf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.havefunace.top/gtvgdjfovh.html

[S60] C++：遍历并删除元素
来源：http://hz.hnxiangtu.top/gtfjhcufih.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuanzhike.top/gtnuwhsbff.html

================================================================================
来源：http://hz.hysaishi.cn/gtyiwfyxar.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cdnleiting.top/gtqdweneqm.html

================================================================================
来源：http://hz.redwolf501.top/gtdtkhodfi.html

[T01] Kotlin：Hello World
来源：http://hz.havefunace.top/gthcymmesk.html

println("Hello")
来源：http://hz.shanyushiyangkeji.top/gtbgttbsph.html

[T02] Kotlin：变量
来源：http://hz.gaohongyu789.top/gtjigjfaes.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.iojbl.cn/gtudurnltf.html

[T03] Kotlin：字符串模板
来源：http://hz.ybcxt.top/gtnheerhba.html

"值: $b"
来源：http://hz.yvedp.cn/gtsdecfedi.html

[T04] Kotlin：空安全
来源：http://hz.snrcjt.cn/gtmousevds.html

val n: String? = null;  n?.length
来源：http://hz.ywan-chungtsiang.top/gtqfrzmfvc.html

[T05] Kotlin：when 表达式
来源：http://hz.nanxuanxn.top/gtnkdeafdb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hysaishi.cn/gtgntrcdox.html

[T06] Kotlin：集合映射
来源：http://hz.gzhubu.top/gtaciwmepa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yj202588.top/gtrvqzpvla.html

[T07] Kotlin：集合过滤
来源：http://hz.fzhhl.top/gtllomshpx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj20258888.top/gtweqriure.html

[T08] Kotlin：数据类
来源：http://hz.jinqigfzy.top/gtgturfkxl.html

data class User(val name: String, val age: Int)
来源：http://hz.andypj.xyz/gtxhwnvmoc.html

[T09] Kotlin：扩展函数
来源：http://hz.hammf.cn/gtybutfpuv.html

fun String.exclaim() = this + "!"
来源：http://hz.ppjwa.cn/gtidtjggsa.html

[T10] Kotlin：默认参数
来源：http://hz.daria6918.cn/gtmhypgupp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.iojbl.cn/gtnndekkew.html

[T11] Kotlin：协程
来源：http://hz.haohaochexian.top/gtjwhhnnzk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhoulong.xyz/gtroovhyul.html

[T12] Kotlin：解构声明
来源：http://hz.tianlin.xyz/gtfbcvfxri.html

val (a, b) = Pair(1, 2)
来源：http://hz.ywan-chungtsiang.top/gtqhwelasi.html

[T13] Kotlin：只读 Map
来源：http://hz.jlsjyb.cn/gtdyroossf.html

val m = mapOf("a" to 1)
来源：http://hz.shzxlz.cn/gthjochejj.html

[T14] Kotlin：循环
来源：http://hz.hnxiangtu.top/gtnnggpwcs.html

for (i in 1..10) println(i)
来源：http://hz.yj20258888.top/gtncmqovrv.html

[T15] Kotlin：接口
来源：http://hz.yuanzhike.top/gtbhctldmz.html

interface Shape { fun area(): Double }
来源：http://hz.hfpthk.cn/gtjarkjxqg.html

[T16] Swift：Hello World
来源：http://hz.guowangkeji.top/gtnzgufcka.html

print("Hello")
来源：http://hz.ybcxt.top/gtqrmbrrpf.html

[T17] Swift：变量与常量
来源：http://hz.shanyushiyangkeji.top/gtkbgdouaa.html

var a = 1;  let b = 2
来源：http://hz.sxryk.cn/gtwunhavdc.html

[T18] Swift：字符串插值
来源：http://hz.cashguo.top/gtnopckcdl.html

"值: \(b)"
来源：http://hz.snrcjt.cn/gtvwxxpwfa.html

[T19] Swift：可选绑定
来源：http://hz.zhiwuduotai.top/gtlffqbyxx.html

if let n = opt { print(n) }
来源：http://hz.jyoumei.cn/gtbcsnmfnz.html

[T20] Swift：数组操作
来源：http://hz.jianghu66.top/gtzgymllpr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.fzhhl.top/gtwdaxdzve.html

[T21] Swift：遍历
来源：http://hz.hnqzz.top/gtmasvigvi.html

for x in a { print(x) }
来源：http://hz.sysykeji.top/gtvaycolzq.html

[T22] Swift：字典
来源：http://hz.iojbl.cn/gtibmafcqc.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.tianlin.xyz/gtkxyvbpms.html

[T23] Swift：函数
来源：http://hz.ehwqpu.com/gtlwksnaqt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.aibaodan.cn/gtfecqdiek.html

[T24] Swift：闭包
来源：http://hz.fengsongda.top/gtlyofyoni.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shangyingyoupin.top/gtojwcnycy.html

[T25] Swift：结构体
来源：http://hz.zycfv.cn/gttebtxhbb.html

struct P { var x: Int }
来源：http://hz.gotoacloud.top/gtsilotlap.html

[T26] Swift：类与重写
来源：http://hz.jqgfzy.top/gtlibjyupa.html

class A: Base { override func f() {} }
来源：http://hz.zhoulong.xyz/gthnhgpgac.html

[T27] Swift：错误处理
来源：http://hz.jianghu66.top/gtcknvozze.html

do { try f() } catch { print(error) }
来源：http://hz.shanyushiyangtech.top/gtatgggmus.html

[T28] Swift：枚举
来源：http://hz.fzhhl.top/gtzjcdtnxd.html

enum Color { case red, green }
来源：http://hz.xuetiantiany.cn/gtbtdnmjnn.html

[T29] Swift：guard 提前返回
来源：http://hz.wangshuangyany.cn/gthtqhkkhn.html

guard let x = opt else { return }
来源：http://hz.nwbrower.top/gtzwlljyru.html

[T30] Swift：协议
来源：http://hz.shanyushiyangtech.top/gtfrpszrwc.html

protocol Shape { func area() -> Double }
来源：http://hz.guannengcc.top/gtmzscceqe.html

[T31] Lua：Hello World
来源：http://hz.cheryme.top/gtjxfhitcf.html

print("Hello")
来源：http://hz.sxryk.cn/gtrlsqangy.html

[T32] Lua：局部变量
来源：http://hz.tianlin.xyz/gtdqrjakdd.html

local a = 1
来源：http://hz.meibo888.top/gtycucccgt.html

[T33] Lua：表（数组）
来源：http://hz.cucudq.cn/gtmdbsojat.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.nwbrower.top/gticprxoxb.html

[T34] Lua：遍历表
来源：http://hz.yj20258888.top/gtpdsxpopj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.svipenyu.cn/gtkgzkmebm.html

[T35] Lua：字典表
来源：http://hz.ehwqpu.com/gtgugqmwtn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhoulong.xyz/gtuhixerpu.html

[T36] Lua：函数
来源：http://hz.xinyue.icu/gtcjpmgzfi.html

function add(a, b) return a + b end
来源：http://hz.smart0.xyz/gtqgmvzyyl.html

[T37] Lua：字符串拼接
来源：http://hz.hfpthk.cn/gtxlckfixa.html

"a" .. "b"
来源：http://hz.yanxiufei.cn/gtmehqombp.html

[T38] Lua：条件
来源：http://hz.zhijiandao.cn/gtwcqefzkh.html

if x > 0 then print("正") end
来源：http://hz.xuanzx.com/gtggwasoai.html

[T39] Lua：模式匹配
来源：http://hz.ybcxt.top/gtwjvichdx.html

string.find(s, "%d+")
来源：http://hz.jqgufenzy.top/gtnwuvjdpv.html

[T40] Lua：元表
来源：http://hz.gotoacloud.top/gtdgdwdvcu.html

setmetatable({}, { __index = base })
来源：http://hz.sxryk.cn/gtbwwoqcmc.html

[T41] Perl：Hello World
来源：http://hz.hammf.cn/gtecvydekv.html

print "Hello\n";
来源：http://hz.xuetiantiany.cn/gtcarszhff.html

[T42] Perl：变量类型
来源：http://hz.wangshuangyany.cn/gtzwtmxmsm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.0kj1m.cn/gtmcejcmum.html

[T43] Perl：字符串插值
来源：http://hz.chenjidiqi.icu/gtgoyfglvw.html

"值: $a"
来源：http://hz.svipenyu.cn/gtqgzwjlyt.html

[T44] Perl：条件
来源：http://hz.birdmap.top/gtduoeoxek.html

if ($a > 0) { print "正"; }
来源：http://hz.svipenyu.cn/gthdvmcqxx.html

[T45] Perl：数组遍历
来源：http://hz.aizwys.cn/gtkxjczubb.html

for my $x (@arr) { print $x; }
来源：http://hz.zhixingplan.top/gtwtromrye.html

[T46] Perl：哈希操作
来源：http://hz.dashuyun.cn/gtbkyuoxsh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.gaohongyu789.top/gtlofynhao.html

[T47] Perl：正则捕获
来源：http://hz.ybcxt.top/gtipyoyjtn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.gogol.net.cn/gtgbehxfig.html

[T48] Perl：正则替换
来源：http://hz.birdmap.top/gtdmzpoiom.html

$s =~ s/old/new/g;
来源：http://hz.yj20258.top/gtkwriqqdm.html

[T49] Perl：函数
来源：http://hz.chenjidiqi.icu/gtdrncsdci.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.snrcjt.cn/gtpnizrtxi.html

[T50] Perl：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtxmnnnira.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.redwolf501.top/gtchqtboby.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ywan-chungtsiang.top/gtavieukuz.html

[T51] Scala：Hello World
来源：http://hz.jinghuilouyu.cn/gtfenrmejd.html

println("Hello")
来源：http://hz.haohaochexian.top/gtteuqdwdi.html

[T52] Scala：变量
来源：http://hz.ybcxt.top/gtclvigxeg.html

val a = 1;  var b = 2
来源：http://hz.xylfe.cn/gtvitwfxok.html

[T53] Scala：字符串插值
来源：http://hz.haohaochexian.top/gtlpmbyggi.html

s"值: $b"
来源：http://hz.nanxuanxn.top/gttqrpaouj.html

[T54] Scala：集合映射
来源：http://hz.0kj1m.cn/gtpqpygztt.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.c1oappe.top/gtomrmwvbt.html

[T55] Scala：集合过滤
来源：http://hz.andypj.xyz/gtycskstwl.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.chenlongwang.top/gtokydhzuh.html

[T56] Scala：样例类
来源：http://hz.yangfankeji.com/gtmgisxkur.html

case class User(name: String, age: Int)
来源：http://hz.guowangkeji.top/gtxhqqndtw.html

[T57] Scala：模式匹配
来源：http://hz.xziqi.cn/gtuujhrhbz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.pengpengdd.cyou/gtpviymztm.html

[T58] Scala：函数定义
来源：http://hz.chenjidiqi.icu/gtzmyepxeg.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.guowangkeji.top/gtwopchxtv.html

[T59] Scala：循环
来源：http://hz.yanxiufei.cn/gtxqmmoyuj.html

for (i <- 1 to 10) println(i)
来源：http://hz.gaohongyu789.top/gtitkqqtue.html

[T60] Scala：折叠
来源：http://hz.pengpengdd.cyou/gtirxfsrhy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jianghu66.top/gtjbyxqgka.html

================================================================================
来源：http://hz.yanxiufei.cn/gtoxvtcuym.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.gzhubu.top/gtozzdwpcy.html

================================================================================
来源：http://hz.cheryme.top/gtyayaudok.html

[U01] Py：创建虚拟环境
来源：http://hz.dianchejie.cn/gtjvtsvpdl.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.smart0.xyz/gtcpfpavyu.html

[U02] Py：导出 / 安装依赖
来源：http://hz.sufxvd.cn/gtugnyoell.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.daria6918.cn/gteekvkfdr.html

[U03] Py：加载 .env 配置
来源：http://hz.shuidangran.top/gttgtjmodj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.nanxinkj.top/gtoxsxwjqy.html

[U04] Py：变量调试打印
来源：http://hz.wangshuangyany.cn/gtlofpopsg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hysaishi.cn/gtqqnmryys.html

[U05] Py：列表去重且保序
来源：http://hz.xinyue.icu/gtsqenqkgu.html

list(dict.fromkeys(arr))
来源：http://hz.bjfxy.top/gtqjkunamk.html

[U06] Py：合并两个字典
来源：http://hz.aibaodan.cn/gtgvdlgvme.html

{**a, **b}
来源：http://hz.zhiwuduotai.top/gtibinxbjg.html

[U07] Py：反转字典键值
来源：http://hz.vqdsnc.cn/gtqttkifrs.html

{v: k for k, v in d.items()}
来源：http://hz.hammf.cn/gtpxvnfkrp.html

[U08] Py：展平二维列表
来源：http://hz.316326.xyz/gttisdiskp.html

[y for x in nested for y in x]
来源：http://hz.ydzc1.top/gtgfxlnshn.html

[U09] Py：字典取最大值的键
来源：http://hz.wangshuangyany.cn/gtsiyrjizc.html

max(d, key=d.get)
来源：http://hz.xuanzx.com/gtaqmbtogx.html

[U10] Py：按值排序字典
来源：http://hz.yj20258.top/gtfbvdjrve.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.52xcode.cn/gtyvrqsggl.html

[U11] Py：生成器表达式
来源：http://hz.chenzaomai.com/gtmuifebmc.html

(x * 2 for x in arr)
来源：http://hz.zhongyouzk.top/gtimjnbsdb.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jyoumei.cn/gtptszebxl.html

Counter(arr).most_common(3)
来源：http://hz.52xcode.cn/gtpdordbxt.html

[U13] Py：固定长度队列
来源：http://hz.yuxming.cn/gthcpgnqbt.html

deque(maxlen=10)
来源：http://hz.zhongyouzk.top/gtwoenghkk.html

[U14] Py：分组收集到列表
来源：http://hz.hnqzz.top/gtyictsiyr.html

defaultdict(list)
来源：http://hz.hnxiangtu.top/gtkmoacetz.html

[U15] Py：高精度计时
来源：http://hz.chenzaomai.com/gtsyhoabtc.html

t = time.perf_counter()
来源：http://hz.shanyushiyangtech.top/gthxirqvmj.html

[U16] Py：命令行参数解析
来源：http://hz.zhiwuduotai.top/gtuniwpojh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.birdmap.top/gtehcudrmb.html

[U17] Py：初始化日志
来源：http://hz.zhengqikj.top/gtzzffoery.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.nanxinkj.top/gtgqlunvpv.html

[U18] Py：预编译正则
来源：http://hz.gogol.net.cn/gtrgrirepg.html

pat = re.compile(r"\d+")
来源：http://hz.wangdashe.top/gtmnvpkiil.html

[U19] Py：正则替换带回调
来源：http://hz.dianchejie.cn/gtarkscdnx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yuxming.cn/gttlwcqlnb.html

[U20] Py：缓存函数结果
来源：http://hz.ybcxt.top/gtypuqvlqr.html

@functools.lru_cache(maxsize=None)
来源：http://hz.iojbl.cn/gtueflejqn.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhoulong.xyz/gtwzpvwmki.html

@contextlib.contextmanager
来源：http://hz.sweek.top/gtzvtwerqp.html

[U22] Py：矩阵转置
来源：http://hz.zhijiandao.cn/gtbjokvisd.html

list(zip(*m))
来源：http://hz.birdmap.top/gtjfedawrc.html

[U23] Py：分块读取大文件
来源：http://hz.chenzaomai.com/gtxcxctoyk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yueranfly.top/gtpsvonltu.html

[U24] Py：路径操作
来源：http://hz.yongpay.top/gtyxhuuueb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.birdmap.top/gtppiueybz.html

[U25] Py：CSV 按字典读
来源：http://hz.316326.xyz/gtbykzmzmz.html

csv.DictReader(f)
来源：http://hz.nanxinkj.top/gtmfzqtdwx.html

[U26] Py：并发下载
来源：http://hz.jyoumei.cn/gtgacukrhe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.cashguo.top/gteqdznevr.html

[U27] Py：异步 HTTP
来源：http://hz.zhengqikj.top/gtgazijmke.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.cashguo.top/gttpzvxnjg.html

[U28] Py：类型别名
来源：http://hz.jianghu66.top/gtjoswjhsx.html

UserId = int
来源：http://hz.ybcxt.top/gtxvicetze.html

[U29] Py：属性校验
来源：http://hz.svipenyu.cn/gtxtlffkfc.html

@property 与 @x.setter 配合
来源：http://hz.svipenyu.cn/gtledrpovv.html

[U30] Py：数据类
来源：http://hz.tianlin.xyz/gtyuvukapi.html

@dataclass(slots=True)
来源：http://hz.wangshuangyany.cn/gtuzrdvuek.html

[U31] Py：单测
来源：http://hz.cdnleiting.top/gthbymuprt.html

python -m pytest -q
来源：http://hz.hnxiangtu.top/gtbweeolrn.html

[U32] Py：代码格式化
来源：http://hz.chenzaomai.com/gtrenijrmw.html

ruff format . && ruff check --fix .
来源：http://hz.zhaomingkeji.xyz/gtuctknqou.html

[U33] Py：打包发布
来源：http://hz.zhixingplan.top/gtajtgrfon.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.daxiang520.top/gtfnyacxki.html

[U34] Py：判断编码
来源：http://hz.gaohongyu789.top/gtmusgscrf.html

chardet.detect(raw)
来源：http://hz.dashuyun.cn/gtzoifqnzb.html

[U35] Py：发送邮件
来源：http://hz.redwolf501.top/gtiwkfeeom.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xylfe.cn/gttuvujena.html

[U36] Py：定时任务
来源：http://hz.chenjidiqi.icu/gtlmcfdekl.html

schedule.every(10).minutes.do(job)
来源：http://hz.xingfuxueyuan.xyz/gteniwuyko.html


<!-- 参考信息 -->